Frontend Project 4 - Website Performance Optimization

This project consisted of the following parts:

1.) optimize index.html to have a page speed index above 90
2.) make the pizza.html render with 60 FPS when scrolling
3.) make the pizza change sizes using the slider in 5ms or less

Regarding the first task I did:
* minify the print and style css files
* resized and / or compressed images (2048_thumb.png, profile.png, pizzeria_thumb.png)
* add async to scripts
* changed markup to load new optimized images

Regarding the second task I did:
* reduced the number of pizzas created to 30
* minified the main.js file
* moved variables that only need to be calculated once out of the respective loops (scrollTop, items)

Regarding the third task I did:
* refactored the function changePizzaSizes
  * querying for all ".randomPizzaContainer" outside the loop
  * calculating dx outside the loop based on the first element
  * calculating the new width outside the loop
  * calculating length of the pizza container outside the loop
  * only setting the new width inside the loop

Ressources
PageSpeed Insights
Chrome Developer Tools
CSS minifier http://cssminifier.com/
JS minifier http://jscompress.com/


