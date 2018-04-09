## Website Performance Optimization portfolio project

### Getting started

This project is hosted on GitHub. You can link to the live files at:
[Web Optimization Project]( https://business-art-technology-man.github.io/frontend-nanodegree-mobile-portfolio/)

#### Part 1: Optimize PageSpeed Insights score for index.html

I did not use a task manager for this project. 
I used the "Webp" image file format to compress files and I resized the images to the size they were being scaled to in the HTML. I also removed CSS which was scaling images inline on the elements. 

I used the "rel" attribute in the "link" element for loading fonts, javascript and style sheets to improve load times. 

I inlined the "style.css" into the index.html because it was small and eliminated an extra download. 

#### Part 2: Optimize Frames per Second in pizza.html

I updated the functions changePizzaSizes and updatePositions to separate reading and calculating from writing styles. By separating the writing of the style information you avoid forced layout and keep the javascript>styles>layout>composite>paint pipeline from looping on itself.

Other optimizations included making sure the background, pizza graphics and content were on appropriate layers to allow the browser to composite the page efficiently. 
