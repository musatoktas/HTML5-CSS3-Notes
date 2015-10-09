#CSS Selectors
We've used a number of HTML elements as CSS selectors so far: we've styled the HTML tags `<h1></h1>` with the CSS selector `h1`, `<p></p>` with `p`, and so on.

You may have guessed this, but if not, we'll say it outright: any HTML element can be a CSS selector! You can modify `<ul>`s, `<table>`s, and even the entire `<body>` by selecting `ul`, `table`, and `body`, respectively.

For instance you can change your background color by using CSS selector very simply. There it is;
Open your stylesheet.css page and wirte down these simple codes:

    body{
    	background-color: purple
    }

After this you'll seethat your webpage background color become purple.

###What if nest HTML elements inside one another?
For example you want to edit your header inside 2 `<div>` by using CSS. But how can you do that? There is your answer;

here is our code which is we want to edit:
    
    	   <div>
    			<h3>Me, too!</h3>
    			<div>
    				<h3>Me three!</h3>
    				<div>
    					<h3>Forget you guys. I'm about to be red!</h3>
    				</div>
    			</div>
    		</div>
    
I want to edit  `<h3>Forget you guys. I'm about to be red!</h3>` part right?

    div div div h3{
    
    	color: red
    }
###What if I want to edit all elements in the HTML page?
There is our universal selector `*`. If you use this code in the stylesheet.css you mean that you choose every single selectors which you use in your HTML page.
 
There it is; ![](http://s12.postimg.org/excgf19wd/Universal_Selector.png)

###What if way is too long?

Good work! Let's try something a little more involved.

Remember, you can reach an element that is a child of another element like this:
 ` div div p { /* Some CSS */ }`
where in this case, we'd be grabbing any `<p>` that is nested somewhere inside a `<div>` that is nested somewhere inside another `<div>`. If you want to grab direct children—that is, an element that is directly nested inside another element, with no elements in between—you can use the `> `symbol, like so:
  `div > p { /* Some CSS */ }`
This only grabs `<p>`s that are nested directly inside of `<div>`s; it won't grab any paragraphs that are, say, nested inside lists that are in turn nested inside `<div>`s.

##Going to More More Deeper
Alright guys there are a couple of useful selectors right here. Classes and IDs. They are mean that specifical address of the editing.There are also two important selectors you can use in addition to the universal selector and HTML elements: classes and IDs.
###1.Classes
Classes are useful when you have a bunch of elements that should all receive the same styling. Rather than applying the same rules to several selectors, you can simply apply the same class to all those HTML elements, then define the styling for that class in the CSS tab.

Classes are assigned to HTML elements with the word class and an equals sign, like so:
    
    <div class="square"></div>
    <img class="square"/>
    <td class="square"></td>
Classes are identified in CSS with a dot (.), like so:

    .square {
    	height: 100px;
    	width: 100px;
    }
This allows you to take elements of different types and give them the same styling.

###2. IDs
IDs, on the other hand, are great for when you have exactly one element that should receive a certain kind of styling.

IDs are assigned to HTML elements with the word id and an equals sign:

    <div id="first"></div>
    <div id="second"></div>
    <p id="intro"></p>
IDs are identified in CSS with a pound sign (`#`):

    #first {
    height: 50px;
    }
    
    #second {
    height: 100px;
    }
    
    #intro {
    color: #FF0000;
    }
This allows you to apply style to a single instance of a selector, rather than all instances.

###Pseudo Class Selector
This is very cool element of CSS. It's effect HTML elements when you move mouse sign on it or when you click on it. Here more informations are coming. You've learned about class selectors. Now it's time to learn about pseudo-class selectors.

A pseudo-class selector is a way of accessing HTML items that aren't part of the document tree (remember the tree structure we talked about earlier?). For instance, it's very easy to see where a link is in the tree. But where would you find information about whether a link had been clicked on or not? It isn't there!

Pseudo-class selectors let us style these kinds of changes in our HTML document. For example, we saw we could change a link's text-decoration property to make it something other than blue and underlined. Using pseudo selectors, you can control the appearance of unvisited and visited links—even links the user is hovering over but hasn't clicked!

The CSS syntax for pseudo selectors is

    selector:pseudo-class_selector {
    property: value;
    }
It's just that little extra colon (`:`).

##### <div style="width:450px; height:25px; background-color:yellow"> An Useful Note Right Here - - - > Links of Pseudo-class Selector</div></a>
There are a number of useful pseudo-class selectors for links, including:

- `a:link:` An unvisited link.
- `a:visited:` A visited link.
- `a:hover:` A link you're hovering your mouse over.
- `a:active:` A link which is you selecting. 
You can try from this url;
[http://www.w3schools.com/css/tryit.asp?filename=trycss_link](http://www.w3schools.com/css/tryit.asp?filename=trycss_link)

- <em>Children</em> There is also one more useful pseudo-class selector is `first-child`. Is choosing first child of the parents. There is a first child example;
<img src="http://s4.postimg.org/h7jfgqnod/First_child.png"/> 

Here is the CSS code which I wrote in the stylesheet.css to edit first-child;

    p:first-child{
    font-family: Cursive
    } 

and it will be appear like this;

<p style="font-family: cursive"><strong>I'm the first child!</strong></p>



You may edit first child by using `first-child` pseudo-class selector.

You can also try it yourself by following this link: <a href="http://www.w3schools.com/cssref/tryit.asp?filename=trycss_sel_firstchild"><u>first-child try it youself</u></a>

- I can feel your thoughts like, what of we want to choose nth child? May we edit it? Yes you may!! You can actually select any child of an element after the first child with the pseudo-class selector `nth-child`; you just add the child's number in parentheses after the pseudo-class selector. For example,

        p:nth-child(2) {
    		color: red;
    	}
Would turn every paragraph that is the second child of its parent element red.

The element that is the child goes before `:nth-child`; its parent element is the element that contains it. There is an important hint! There is no space between `p:` and `nth-child`.



##So far So Good!!

Great work! So far in this course, you've learned:

- A wider range of CSS selectors
- About cascading
- The universal selector
- Class and ID selectors
- Pseudo selectors


See you on the next lesson! Just Keep Moving to Workingggg!