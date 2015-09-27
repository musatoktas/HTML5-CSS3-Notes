# Welcome to CSS #

----------

Finally we learn basics about HTML! Now we can able to learn CSS(Cascading Styling Sheets.) It's working for making up our HTML files. Its like skin on the bones. Our webpage bones are HTML, and skin is CSS. 

In CSS lessons, we will overlook on CSS, after  we'll go deep inside in it. First of all we are writing our CSS codes in `stylesheet.css` page which is beside our `index.html` page. Lets start on `<span>`s which I refered before in *HTML-CSS Basics-III* lesson.

####Talk a little bit more about `<span>-</span>`
`<span>-</span>` s are simply working for apply similar appearance and formatting to several HTML pages from a single CSS file. 
####Where HTML page get CSS codes
We understand that HTML and CSS are working together to occur Webpage, but we aren't writing CSS and HTML at the same editor. So where HTML page get CSS codes?
There are two ways to put CSS in one page.

**1.** Writing down all of in `<head>-</head>` tags, I mean, Inside the head of HTML page, by using `<style>-</style>` tags. Here is an example about it.
    
        <head>
    		<style>
    			p {
    				color: purple;
    			}
    		</style>
    		<title>Result</title>
    	</head>
    

**2.** But there's an even better way.

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