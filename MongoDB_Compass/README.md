# How to install Dark Mode in MongoDB Compass

> NOTE: make sure you have latest NodeJS and NPM installed on your machine

The following steps would be for Linux but replicating it on Windows should be similar

1. First locate the directory where MongoDb Compass is installed, in most cases it is 
   ```console
   $ cd /usr/lib/mongodb-compass/resources
   ```

2. run 

   ```console
   $ sudo npx asar extract app.asar dest_dir
   ```

3. Add a new JavaScript file in `dest_dir/src/app` called `darkreader.js` and paste the contents of [this file](https://github.com/VolksRat71/environment/tree/main/MongoDB_Compass/darkreader.js) inside of it.

4. find an index.html in the same directory and add the following lines just before `</body>`:

   ```html
   <script src="darkreader.js" charset="UTF-8" async></script>
   ```
5. Save all the changes then cd into `dest_dir` run 

   ```console
   $ sudo npx asar pack . app.asar
   ```

   this will pack the code back into an .asar file

6. Backup the `app.asar` inside /usr/lib/mongodb-compass/resources and then run 

   ```console
   $ sudo mv app.asar /usr/lib/mongodb-compass/resources
   ```

7. Restart Compass and enjoy the theme :)