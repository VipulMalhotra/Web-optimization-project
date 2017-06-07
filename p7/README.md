WEBSITE PERFORMANCE OPTIMIZATION PORTFOLIO PROJECT:
  1.To view the portfolio website download all the files and open index.html in your browser.

  2.To view the pizza website download all of the files and open views/pizza.html in your browser.

  3.In this project we have increase the speed of web pages so that they can load faster by inlining the css in the index.html.
  
  4.In this project we have to render the javascript to optimize our website.
  
  
OPTIMIZATION TO INDEX.HTML PAGE:
  
 Inlined all of the CSS into the head of the document and added the HTML media="print" attribute to the external style sheet link for print styles.
  
OPTIMIZATION TO PIZZA SITE:

1.Modified the code to calculate the number of pizzas needed to fill the webpage based on browser inner dimensions.

2.Moved the document.body request out of for loop in the changePizzaSizes and updatePositions functions. This prevents the browser from having to render the page every time the loop iterates.

3.Cached the needed DOM elements so that the brower isn't querying the DOM every time the for loops are iterated in the updatePositions and changePizzaSizes funcitons

4.Changed all instances of querySelector to the more efficient getElementById and getElementByClassName depending on whether a class or id is needed.

5.In the changePizzaSizes function I created an additional for loop for setting the element's width. This was done to group all of the DOM calls and the Rendering together in separate loops. This prevents the browser from having to render the page over and over in between setting the styles.