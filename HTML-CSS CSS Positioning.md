#CSS Positioning

----------
##Display Property
Its working detect a postion in your web page for your tables, list items, or `<div>`s, etc. You can use a couple of values for this property, we will focus on tree different values of `display:`; inline-block, inline, and none.
###1) `display: inline-block;` Value
Displays an element as an inline-level block container. The inside of this block is formatted as block-level box, and the element itself is formatted as an inline-level box. Basicly its works for list items generally, for example you listed 4 of list item but you want to see them in the one line. So you may take them into the one line using this property. Here is a what Im trying to say;

    <!DOCTYPE html>
    <html>
     <head>
      <style>
       li {
     	display: inline;
    	}
      </style>
     </head>
     <body>
      <ul>
       <li><a href="https://www.google.com">Search</a></li>
       <li><a href="https://www.google.com">Search</a></li>
       <li><a href="https://www.google.com">Search</a></li>
      </ul>
     </body>
    </html>
We used Our property between `<style></style>` blocks.
It will show up on the screen like this
[search.](http://www.google.com "search")[search.](http://www.google.com "search")[search.](http://www.google.com "search")

###2)`display: inline;` 
The inline-block value allows you to put several block elements on the same line. The inline value places all your elements next to one another, but not as blocks: they don't keep their dimensions.
###3)`display: none;` 
Finally, we'll try out the display value `none`. As you might expect, this prevents the page from displaying the selected element. As you might not expect, this removes the selected element from the page entirely, including any children and any content. Poof! Gone! (But not gone forever—changing the display value away from none will bring everything back.)

## Margins, Borders, and Padding 
Now that you understand more about the display property and the box model, we can delve into the details of how each individual box behaves.

Check out the diagram on the below the paragraphs. As you can see, each box is made of layers. From the outermost to the innermost:


1.  The **margin** is the space around the element. The larger the margin, the more space between our element and the elements around it. We can adjust the margin to move our HTML elements closer to or farther from each other.

- The **border** is the edge of the element. It's what we've been making visible every time we set the border property.

- The **padding** is the spacing between the content and the border. We can adjust this value with CSS to move the border closer to or farther from the content.

- The **content** is the actual "stuff" in the box. If we're talking about a `<p>` element, the "stuff" is the text of the paragraph.

You'll see abbreviations like TM, TB, and TP in the diagram. These stand for "top margin," "top border," and "top padding." As we'll see, we can adjust the top, right, left, and bottom padding, border, and margin individually.

<img src="https://s3.amazonaws.com/codecademy-blog/assets/ae09140c.png"/>

###1) Margins
Let's start with our margins. Adjusting our margins not only moves our element relative to other elements on the page, but also relative to the "walls" of the HTML document.

For instance, if we take an HTML element with a specific width (such as our `<div>` in the editor) and set its margin to auto, this tells the document to automatically put equal left and right margins on our element, centering it on the page. Her is what I wrote for an example, and there also a link bottom of the margin code, you can try from their by yourself:
	div {
	height: 50px;
	width: 100px;
	border: 2px solid black;
	border-radius: 5px;
	background-color: #308014;
	margin: auto;
	}
Here is the link --> [Try](http://www.w3schools.com/css/tryit.asp?filename=trycss_margin_sides "w3 schools")






