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
If you want to specify a particular margin, you can do it like this:

    margin-top: /*some value*/
    margin-right: /*some value*/
    margin-bottom: /*some value*/
    margin-left: /*some-value*/
You can also set an element's margins all at once: you just start from the top margin and go around clockwise (going from top to right to bottom to left). For instance,

    margin: 1px 2px 3px 4px;
will set a top margin of 1 pixel, a right margin of 2, a bottom of 3, and a left of 4.

###2) Borders
We've worked with borders before, but it never hurts to have extra practice. So here is an example;

    div{
    	border: 2px dashed #ff0000	
    }

###3) Padding
Good! Let's adjust the padding. Remember, the padding is the space between your border and your innermost layer: the actual content.

Padding can be set in two ways, just like your margins. You can either select them individually, like this:

    padding-top: /*some value*/
    padding-right: /*some value*/
    padding-bottom: /*some value*/
    padding-left: /*some-value*/
Or select them all in one declaration, like this:

    padding: value value value value;
You should also know that if you want your padding to be the same for all four sides, you can declare that value only once. padding: 10px will give your HTML element 10 pixels of padding on all sides. Like this;

    padding: 10px;
###Negative Values
Did you see that? Your `<div>` got huge! That's because the background color is the same for the content and the padding.

When you give CSS a positive padding or margin value, it puts that space between the element and its reference: for instance, if you have a `<div>` and you give it a margin-left of` 20px,` it puts twenty pixels between the left margin of that `<div>` and the side of the screen. This effectively moves the `<div>` twenty pixels to the right.

If you want to move an element in the other direction, you can give CSS a negative value: `margin-left: -20px` will move the element twenty pixels to the left.

###Review
Cool, right? You can move HTML elements clear off the page with negative margins values.

Time for a quick review to make sure you've got a handle on all this margin and padding stuff!

##Floating
Okay! So we know how our individual elements are constructed. But how do we determine where they go on the page?

One way is to use **floats**. When you **float** an element on the page, you're telling the webpage: "I'm about to tell you where to put this element, but you have to put it into the **flow** of other elements." This means that if you have several elements all floating, they all know the others are there and don't land on top of each other.

You can think of the HTML page as sort of like a sea, and floating elements as boats on it: all the boats have positions on the sea, and they all see and steer clear of each other.

(Some of the positioning methods we'll learn in upcoming sections can accidentally drop elements on top of each other.)

###*Clearing Elements

Unfortunately, we sometimes mix large floating elements with non-floating ones, and elements do end up on top of each other.

See your footer (the blue bit between the two columns)? It's stuck back there because we haven't told it something very important: to clear the other elements on the page!

If you tell an element to clear: left, it will immediately move below any floating elements on the left side of the page; it can also clear elements on the right. If you tell it to clear: both, it will get out of the way of elements floating on the left and right!

The syntax is what you're used to:
    
    element {
    clear: /*right, left, or both*/
    }
##Absolute Positioning
The first type of positioning is absolute positioning. When an element is set to position: absolute, it's then positioned in relation to the first parent element it has that doesn't have position: static. If there's no such element, the element with position: absolute gets positioned relative to `<html>`.
##Relative Positioning
**Relative** positioning is more straightforward: it tells the element to move relative to where it would have landed if it just had the default static positioning.

If you give an element relative positioning and tell it to have a margin-top of 10px, it doesn't move down ten pixels from any particular thing—it moves down ten pixels from where it otherwise would have been.
##Fixed Positioning##
<strong>Fixed</strong> positioning anchors an element to the browser window—you can think of it as gluing the element to the screen. If you scroll up and down, the fixed element stays put even as other elements scroll past.
Thank you For following my instructions. It was awesome experience for me to. See you on next tutorial.