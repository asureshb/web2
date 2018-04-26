

HTML & CSS (Module 12, Day 2):

- Worked on Activity1 to create simple webpage that displays bio, image, favorites
- Learnt about pages.github.com to create personal websites on github.com domain,
  also showcase personal projects on github pages from github repositories.

- Activity2: created website repo on github pages:
		https://asureshb.github.io

- Copied bio html to this repo to display bio on github pages

- Activity3: Created an index.html page under one of my projects on github,
changed the project settings to make github pages use master as source,
now the project documentation is accessible via github pages:

https://asureshb.github.io/RealEstate_DataAnalysis/

- Read through the slides to learn basics of CSS:
https://ucb.bootcampcontent.com/UCB-Coding-Bootcamp/UCBBEL201801DATA5-Class-Repository-DATA/blob/master/12-Web/2/Slide-Shows/CSS_Stylin.pptx

- CSS (Cascading Style Sheet) is used to format/position the elements on webpage
- HTML is to create the content of webpage where as CSS is to structure the elements
on webpage.

- CSS gives flexibility to change and style fonts at pixel level and also position
headers, text, images as required.

- CSS properties (like font, size, color, background) can be defined as a class
and pass name of that class as a property to the HTML element, 
so that those properties are applied to those elements on webpage.

- CSS Box Model:
In terms of webpage design and layout, every element on webspage is considered as a box

Explanation of the different parts:

Content - The content of the box, where text and images appear
Padding - Clears an area around the content. The padding is transparent
Border - A border that goes around the padding and content
Margin - Clears an area outside the border. The margin is transparent

Example:
div.<position> {
    position: <position>;
    width: 300px;
    border: 25px solid green;
    padding: 25px;
    margin: 25px;
}

Position types:
 - Static (default)
 - relative
 - absolute
 - fixed
 - sticky

- Layering (overlapping of boxes) with Z-Index:
when elements on the webpage are positioned, they can overlap sometimes.
Z-Index is a property that decides where to position element in the stack.
Elements with negative/lowest z-index go behind and
elements with positive/highest z-index are placed at the front.

Eg:
img {
    position: absolute;
    left: 0px;
    top: 0px;
    z-index: -1;
}


-Hiding elements: This helps to display or hide the content dynamically
Eg:
.box-1: {
    display: none;
}

- Flow & Float:
  - By default HTML elements uses 'Flow' mechanism, every block of HTML element takes entire line of space
  - Float is a CSS property used to position multiple elements inline
  
  Eg:
  box1 {
      float: left;
  }
  
  box2 {
      float: right;
  }


- Clearfix Hack:
    Clear fix is a technique to automatically resize the floating container/box that matches elements in it
    
    .clearfix {
    	overflow: auto;
	}


    Following example clear fixes the container/box after all the elements and content are positioned
	.clearfix::after {
    	content: "";
    	clear: both;
    	display: table;
	}
