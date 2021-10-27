# Introduction

###

So I used Mongodb Compass for a little time a few months ago and then i switched to another mongo client gui for the sole reason, Darkmode.
That mongo client was good but recently it became paid. I then switched back to Compass but my eyes couldnt take it 😩

Then I spent some time researching what could I do to make compass darker and easier to read and I found this [npm package](https://www.npmjs.com/package/darkreader) for the Darkreader chrome plugin.
I knew that compass was made in Electron as it had `.asar` files in its source, that means I could easily implemt that npm package into the Electron app.

Here is the result!
![preview](https://cdn.discordapp.com/attachments/840902589620944907/900968619675099166/unknown.png)

# How to

###

> make sure you have latest NodeJS and NPM installed on your machine

The following steps would be for linux but replicating it on windows would be easy too

1. First locate the directory where MongoDb Compass is installed, in my case it is `/usr/lib/mongodb-compass`, cd into the `resources` directory

2. run `npx asar extract app.asar dest_dir`

3. Add a new JavaScript file in `dest_dir/src/app` called `darkreader.js` (you change the name too) and paste the contents of [this file](https://unpkg.com/darkreader@4.9.39/darkreader.js) inside it.
   append these lines of code at the very end of the file:
   ```js
   DarkReader.enable({
       brightness: 100,
       contrast: 90,
       sepia: 20
   });
   ```
   you can ofc play with these values to get the taste you want.

4. find an index.html in the same directory and add the following lines just before `</body>`:
   ```html
   <script src="darkreader.js" charset="UTF-8" async></script>
   ```
5. save all the changes then cd into `dest_dir` run `npx asar pack . app.asar`, this will pack the code back into an .asar file
6. Backup the `app.asar` inside /usr/lib/mongodb-compass/resources and then run `mv app.asar /usr/lib/mongodb-compass/resources`
7. Restart Compass and enjoy the theme :)