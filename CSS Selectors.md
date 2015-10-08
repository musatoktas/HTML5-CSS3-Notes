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