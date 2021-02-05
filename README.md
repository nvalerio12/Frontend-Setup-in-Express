Frontend Setup in Express\

Setup

0.
Do a basic express app setup. If you need step by step instructions, look at one of our previous lessons. You should install the npm packages express, ejs, and express-ejs-layouts


Add a home route that renders an index.ejs file with some text, and put some boilerplate HTML in our layout.ejs page with that special <%- body %> tag.

1.
Set up your static files and folder structure.

Create public folder in top level folder
Put the following line of code in your server index.js
This is some middleware that allows us to find static assets like images, css, frontend js, in the public folder.
app.use(express.static(__dirname + '/public/'));
Inside the public folder, create folders css, js, images.

2.
Create some frontend files and place them in the appropriate file. You'll need a style.css file, a main.js file, and pick a random image from the internet or your computer to copy into the images folder.

3.
Link the CSS file

in the head of layout.ejs file, add the line:
<link rel="stylesheet" href="css/style.css">
add a style rule to the CSS file to test the connection. Something like this:
```
body {
    background: goldenrod;
}
``
If you don't see the background colour change in your browser, check the href attribute of the link tag, then make sure the CSS file was saved, then make sure the express.static() line from step 1 is copied exactly. You got this!

4.
Link the JS file and add a console.log to make sure it is working. Remember script src.

Then display the image in an <img /> element added to index.ejs.

Take 5 min. and use what you know so far to try and figure it out and don't forget to use the docs or other resources. We'll take this up as a class afterward.
