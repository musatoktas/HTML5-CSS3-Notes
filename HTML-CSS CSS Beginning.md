# Welcome to CSS #

----------

Finally we learn basics about HTML! Now we can able to learn CSS(Cascading Styling Sheets.) It's working for making up our HTML files. Its like skin on the bones. Our webpage bones are HTML, and skin is CSS. 

In CSS lessons, we will overlook on CSS, after  we'll go deep inside in it. First of all we are writing our CSS codes in `stylesheet.css` page which is beside our `index.html` page. Lets start on `<span>`s which I refered before in *HTML-CSS Basics-III* lesson.

#### Talk a little bit more about `<span>-</span>`
`<span>-</span>` s are simply working for apply similar appearance and formatting to several HTML pages from a single CSS file. 
##1. Where HTML page get CSS codes
We understand that HTML and CSS are working together to occur Webpage, but we aren't writing CSS and HTML at the same editor. So where HTML page get CSS codes?
There are two ways to put CSS in one page.

**A.** Writing down all of in `<head>-</head>` tags, I mean, Inside the head of HTML page, by using `<style>-</style>` tags. Here is an example about it.
    
        <head>
    		<style>
    			p {
    				color: purple;
    			}
    		</style>
    		<title>Result</title>
    	</head>
    

**B.** But there's an even better way.

You know you should write your CSS in a totally separate file. But how do you make sure your HTML file can see that CSS information?

You do this by putting a `<link>` tag (as you saw in the first exercise of this course) between the `<head>...</head>` tags of your HTML page. Your `<link>` tag needs three attributes:

A `type` attribute that should always be equal to `"text/css"`
A `rel` attribute that should always be equal to "`stylesheet"`
A `href` attribute that should point to the web address of your CSS file
In the editor to the right, you'll see two files: `index.html` and `stylesheet.css`.

Her is an example;

    <head>
	    <link type="text/css" rel="stylesheet" href="stylesheet.css"/>
		<title>Result</title>
	</head>
After this You can write your CSS codes in `stylesheet.css` page.

##2. Editing Paragraphs

in HTML to edit paragraph we were write codes inside the tags, but in Css we are writing in the `stylesheet.css`, with different way absolutely.
 In html editor our paragraphappearing like this;
  `  <p>`I`'m currently red, but I'm about to become black!``</p> `
To edit our paragraph by CSS, open your `stylesheets.css` and edit what ever you like or want like this;

    p{ 
    	color: red;
    	font-family: Verdana;
    	font-size: 24px;
    }

After your text will show up on your screen like this;

<p style="color: red; font-family: Verdana; font-size: 24px"> I'm currently red, but I'm about to become black!</p>

##### <div style="width:360px; height:25px; background-color:yellow"> An Useful Note Right Here - - - > Comments in CSS</div></a>

In HTML, we were writed down comments like this;
   
 `<!--I'm a comment!-->`

But CSS comments writing styles are completely different than HTML;

    /*I'm a comment!*/

###A. Edit Your Paragraph with Deep Colors 

You've got the main ideas—now it's time to dive into the nitty-gritty.

You've noticed that when we've asked you to set color properties using CSS, we've been having you type things like `color:red`. You may have asked yourself: what if I want maroon? Or fire engine red? Or more of a red-orange? Does CSS know all those words?

The answer is no. It can, however, understand millions of colors in the form of hexadecimal values.

You're already extremely familiar with decimal values: it's everyday counting! You know when you see a number (e.g. 1,432) that each digit can only be the ten values 0 through 9. Because there are only ten possibilities, we say that regular counting is base-10.

Hexadecimal counting is base-16. Each digit can be the numbers 0 through 9 or the letters a through f! Crazy, right? Check it out:
<h1 style="color: #8B1C62">I'm maroon!</h1>
<h2 style="color: #FF7256">I'm coral!</h2>
<h3 style="color: #FFC125">I'm goldenrod!</h3>
<h4 style="color: #54FF9F">I'm sea green!</h4>
<h5 style="color: #530EE8">I'm royal blue!</h5>
<h6 style="color: #8B668B">I'm plum!</h6>

###B. What if Client Using Different Screen?
When we've asked you to adjust font size, we've specified that the unit you should use is px (for "pixels"), like so:

    p {
    font-size: 10px;
    }
A pixel is a dot on your computer screen. Specifying font sizes in pixels is great when you want the user to see exactly on their screen what you designed on yours, though it assumes your screens are of similar size.

What if the user is using a screen that's a very different size from yours, though (like a smartphone screen)? Enter ems. (Don't confuse these with the `<em></em>` tags we use for emphasis!)

The font-size unit em is a relative measure: one em is equal to the default font size on whatever screen the user is using. That makes it great for smartphone screens, since it doesn't try to tell the smartphone exactly how big to make a font: it just says, "Hey, `1em` is the font size that you normally use, so `2em` is twice as big and `0.5em` is half that size!"

Check it out: we've set three different paragraphs to the font-sizes` 1em`, `0.5em`, and `2em`. For now, use whichever unit (px or em) you're more comfortable with—we just wanted to show you em now so you're not surprised when you see it later.

###C. What If Client Computer Hasn't Font Which You Use in  Your Webpage 

You don't have to jump straight to a default value like cursive or sans-serif: you can tell CSS to try several, going from one to the next if the one you want isn't available.

For example, if you write:

    p {
    font-family: Tahoma, Verdana, serif;
    }
CSS will first try to apply , <span style="font-family: tahoma">Tahoma</span> to your paragraphs. If the user's computer doesn't have that font, it will try <span style="font-family: Verdana">Verdana</span> next, and if that doesn't work, it will show a default <span style="font-family: serif">serif</span> font.

#####<div style="width:400px; height:25px; background-color:yellow"> An Useful Note Right Here - - - > Serif, Sans-serif, Curiel</div></a>

**serif:** A font with little decorative bits on the ends of the strokes that make up letters. Do a search on "serif" to see what we mean.

**sans-serif:** A plain-looking font, like this one. It doesn't have the little doohickies on the ends of letters like a serif font does.

**cursive:** A scripty font! It looks like cursive writing.

###Review
Great work! You've learned a ton so far. Let's take a quick breather to review.

We've covered:

- What CSS is
- Why we separate form from function
- CSS syntax, including (multiple) selectors, (multiple) property-value pairs, and comments
- Details of how colors, font sizes, and font families work

##3. Make Your Tables a Little Bit Fancy
 
Many HTML elements support the border property. This can be especially useful with tables.

The border property in turn supports several values. For example, for a border 2 pixels thick, solid, and red, you'd type

    selector {
    border: 2px solid red;
    }
Borders: pretty fancy. It will show up like this;

<table border="2px; color: solid red">
	<thead>
	</thead>
	<tbody>
		<td> Focus on The border of Table</td>
	</tbody>
</table>

##4. Links Decoration
Links have a lot of the same properties as regular text: you can change their font, color, size, and so on.

But links also have a property, text-decoration, that you can change to give your links a little more custom flair. You're probably used to seeing links that are blue and underlined, right? Well, that's not the way it has to be!
You gonna write down in to your `stylesheet.css` page these:

    a{
    color: #cc0000;
    text-decoration: none;
    }
And your link will show up like this:
 <a href="http://www.google.com/">Google</a>

#####<div style="width:425px; height:25px; background-color:yellow"> An Useful Note Right Here - - - > Selectors, Property, Value </div></a>
Let's review selectors, properties, and values. Remember, the syntax is

    selector {
    property: value;
    }
