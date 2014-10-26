# D'Oh! A Donut-y Plug-In

Always dreamed of having donuts rain down on your website with the click of a button? Well, here you go!

## Getting Started

### Browser Support

Unfortunately, this plug-in will __not__ work on FireFox. This is an issue with the jQuery CDN and I am unsure on how this can be fixed. Hopefully it will soon! However, the plug-in works perfectly on both Safari and Chrome browsers. 

### What you will need:

* A URL to the jQuery CDN: [https://ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js]
* Separate folders for both your stylesheets and JavaScript files
* A working knowledge of HTML, CSS, and JavaScript/jQuery

## Step 01:

Download a .zip of the plug-in and save the file.

## Step 02:

Add the "donut.js" file to the folder containing your other JavaScript files. Add the "donut.css" file to the folder containing your other CSS files. Copy all images from the plug-in's images folder to the folder containing your site's images.

## Step 03:

Between the head tags of your HTML file, but after the link tag to your main CSS file, create another link tag leading to the "donut.css" file. Before the closing body tag (but after your main HTML code), include the three following source links in script tags:

* A link to your jQuery CDN (if not included already)
* A link to your main JavaScript file (if not included already)
* A link to the "donut.js" file

## Step 04:

Copy the button tag from the "example.html" file and paste at the end of your own HTML page, before the script and closing body tags.

## Step 05:

From the "main.js" file included with the plug-in, copy and paste line 2 into the function that calls your JavaScript, inside your project's main JavaScript file. Example:

```javascript
$(function(){
	bookApp.init(); //This is calling the main file's script
	$('button').donutRun(); //This is calling the plug-in script
});
```

## Customization

* Replace the donut image files with your own! In line 14 of the "donut.js" file, change the image source to your files' names. Make sure the file names are similar (i.e. cupcake-01, cupcake-02, etc.) and form some sort of sequence (i.e. red, yellow, green, 1, 2, 3, etc.). In the donutClass variable, change the colour strings to match the sequence of your files. Do not alter the "randDonut[i]" value since this will randomize the sequence of the images each time they fall down the page. Make sure the images you use are transparent .png files.

* Alter the speed of the images! In the "donut.css" file, under the "Donut Speeds and Indexes" section, feel free to alter the speed of the images using the webkit-animations provided. I recommend staying with speeds between 2.5 and 9 seconds.

Enjoy! Feel free to fork this and change things around!








