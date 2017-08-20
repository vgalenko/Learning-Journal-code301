# LJ Code 301 - Day 3

Last couple of days I learned about jQuery library and about its many methods. Its amazing to see how you can take 10 lines of vanilla JS code and turn it into 2 lines with jQuery. Ones things is easier to us is 
an event listener/handler. You can target any element, class, id and etc and fire it with .on() handeler method like the example below. 

$( "#someId" ).on( "click", function() {   // when clicked, callback function gets triggered 
  //do stuff here
  //do more suff here 
});

Also helpul methods that I used for last couple days were: 
.find() //it helps to find the descendants of the element 
.text() //displays content into the browser and is better practice then using .html() due to security 
.attr() //Gets the value of an attribute for the first element in the set of matched elements or set one or more attributes for every matched element.
.parent()  //is used if you want to traverse up the DOM tree, very helpful if you're trying to target a parent element. 
