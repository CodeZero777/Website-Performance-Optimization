####Website Performance Optimization portfolio project - Udacity's Nanodegree

###Project Overview

To optimize a provided website with a number of optimization- and performance-related issues so that it achieves a target PageSpeed score and runs at 60 frames per second.

##Instructions:

1) Click the optimized project below:

http://CodeZero777.github.io/Website-Performance-Optimization

2) Test the optimized website above by copying and pasting it into Google's PageSpeed Insights:

https://developers.google.com/speed/pagespeed/insights/

Mobile and desktop scores surpass a score greater than 90.

The original "unoptimized" website that was provided by Udacity took roughly >20 seconds to render on the screen.

You may download the Udacity's original files below: 

https://github.com/udacity/frontend-nanodegree-mobile-portfolio

##Specifications to optimize website:

1) Pagespeed score for the index.html is above 90. Now it is 95. (before: score was ~60 to 70)

2) Pizza.html runs avg. 60 fps. (before it was avg. 15 fps)

3) Resizing pizzas time for pizza.html is <5 ms (~0.49ms)

4) Images where optimized using R.I.O.T. (Radical Image Optimizer Tool) software, and CSS and JS files where minified with http://cssminifier.com and http://javascript-minifier.com.

5) A brief explanations/comments were documented in main.js where the changes were performed.

6) In order to run pizza.html at 60fps certain JS code had to be modified. Thanks to Google's DevTools, it was able to show me where Forced Synchronous Layout (FSL) was occuring. With this information, I moved the code out of the for loop since it was not allowing the site to achieve 60fps, but it was keeping it at 15fps. Another part of the code in main.js, I had to completely modify, so that the resizing of the pizzas was below 5ms. The original was code was resizing the pizza ~140ms.
