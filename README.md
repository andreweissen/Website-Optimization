### Website Optimization ###

#### Andrew Eissen ####

##### About #####
The point of this project was to optimize a portfolio index page and score a PageScore speed of 90 or greater, and optimize a pizza page to run at 60 fps or better.

##### Installation #####
To run, unzip the entire folder. Run "index.html" to examine the portfolio index page, and open the "views" folder and run "pizza.html" to examine the pizza site. 

##### Page Speed Optimizations #####
CSS files were minified and inserted directly into the "index.html" document, with the exception of the "print.css" file, which now utilizes the media tag, calling it for specific instances when the user wants to print the page. Various JS files, now minified, are called and rendered asynchronously as well.

##### FPS Optimizations #####
As before, the bootstrap and styles CSS files have been minified and placed in the html document itself, and the JS file has been minified. As suggested by a Udacity office hours video, various variables, selectors, and length calculators were removed from all "for" loops. Additionally, scroll-related operations were separated into independent functions, and "onScroll" was bound to the event listeners.

Similarly, all instances of "querySelector" and "querySelectorAll" were replaced by "getElementById" and "getElementsByClassName" for increased speed.

Rather than simply rendering 200 pizzas on page load, the height of the screen in pixels is obtained, divided by the number of pixels per row, and multiplied by the number of columns to find the correct number of pizzas to render.

##### Acknowledgements #####
The author was inspired by the GitHub repositories of Rowan Savage, Mike Joyceio, and Allan Breyes, and some bits of their code were reappropriated for this project. Additionally, a number of Google Developer and StackOverflow threads were viewed as resources.

#### Resources ####
- [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/)
- [Udacity Office Hours](https://github.com/udacity/fend-office-hours/tree/master/Web%20Optimization/Effective%20Optimizations%20for%2060%20FPS)
- [CSS Minifier](http://www.cleancss.com/css-minify/)
- [JS Minifier](http://jscompress.com/)
