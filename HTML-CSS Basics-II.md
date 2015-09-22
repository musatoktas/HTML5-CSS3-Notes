#Introduction to the HTML

----------

----------
 
On the previous document I wrote about head and body. Now we will  increase our knowledge about HTML. We will cover these things in this page;


1.  Making ordered and unordered list.
2.  Changing font size, color, and type.
3.  Changing the background color.
4.  Aligning text.


When you coding html, be aware about indentation, which means space between each tags.
##Making Lists

####1-Making an Ordered List:

Making ordered list is very simple. To make an prdered list first of all place a tag `<ol>`. After that write down `<li>-</li>` for each item. Here is an example:
       
    		<h2>List of  things I find just OK</h2>
    		<ol>
    		<li>Studing</li>
    		<li>Singing</li>
    		<li>Flying</li>
    		</ol> 
    	</body>
    	</html>`

####2-Making Unordered List

Whatif I don't wanna making an ordered list? what if I just wanna use bullet points? It's actually very similar to coding onrdered list. Just change `<ol>to <ul>`. Here is an example:

    <ul>
    	<li>Because of my chair</li>
    	<li>Because of my earphone </li>
    	<li>Because of my yatch </li>
    	<li>Because of my keyboard</li>
    </ul> 				

##Adding Comments
Comments start with <!-- and end with --> like this:

    <!-- This is an example of a comment! -->

##Font Size
Recall that `<p>` and `</p>` are opening and closing tags.

We can give tags more instructions by including attributes in the opening tag. An attribute is simply a characteristic or some description for the content in the element. You saw this with src in `<img>` and href in `<a>`.

Let's change the size of the text. How? We use the style attribute. We make it equal to font-size, followed by a colon, the size you want, and end it with px (short for "pixels"). For example:

    <p style="font-size: 12px">

And also here is an example;


	<body>
		<p style="font-size: 10px"> Some text for you to make tiny! </p>
		<p style="font-size: 20px"> Some text for you to make normal size!</p>
		<p style="font-size: 40px"> Some text for you to make super big!</p>
	</body>

##Font Color
What is awesome about the style attribute is that we use it a lot! And we can use it with many different tags, not just `<p>`. Let's now change the colors of our text in a heading.

To change the color of text, simply add the style attribute in the opening tag, then make the style equal to "`color:blue`" (or whatever color you like). For example:


    <h2 style="color:red">
What if you want to change the color and the size of the text? Simple! Just add a semi-colon between each bit. For example:


    <h2 style="color: green; font-size:12px">
A full list of available colors can be found here.

Note: do not type something like:

    <h2 `<h2 style="color: green; font-size:12px">`
If you incorrectly nest your HTML tags like that, your code will not pass.

##Font Style

We've covered font colors and font sizes. But we want more power! We want to decide what font type to use. We can do this using font-family, like this:

    `<h1 style="font-family: Arial">Title</h1`>
First we wrote `<h1>Big title</h1>`
Then inside the opening `<h1>` tag, we added a style attribute, and set it equal to "`font-family: Arial`".
This styles the` <h1> `tag with Arial font.

We can do the same for other tags. So we could have a li:


    <li style="font-family: Arial">Hello!</li>
[Here's a list](http://www.w3.org/TR/CSS21/fonts.html#generic-font-families) of available fonts.



