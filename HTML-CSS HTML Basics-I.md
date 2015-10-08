#Basics of HTML/CSS
---------------------------------------------

Think about WebSites. They have bunch of bridges hypertext. They are writing down with HTML/CSS languages. HTML(HyperText Markup Language) like bones of Websites, and CSS(Cascading Style Sheets) is skin and muscules of Websites. First we have to built skeleton.

1. Things inside `<>`s are called tags.
2. Tags nearly always come in pairs: an opening tag and a closing tag.
3. Example of opening tag: `<html>`
4. Example of closing tag: `</html>`
 
##Head
  Everything on the HTML file writing down between 
`<html></html>` tags. HTML file occuring two parts;head,and body.Lets Start From head! Head Contains information about your html file. Its Like a title of the article. The title is first column of the page like when you see the BBC website title is on the top of the page which is include some logos and shotcuts.
	
  Lets add a head and a title to our webpage.


1.  First of all add our tags`(<html></html>)`
2. Between our tags add an title tags such as`(<html></html>)`
3. Between title tag write down your title of webpage.

there is your webpage title.

##Body

####A. Header 
Lets talk about body. Body is part of the webpage which is include contens for instance; images, links, and texts etc. You can add a paragraph by using `<p>-</p>` tags.
To add Header on the page add`<h1>-</h1>`tags and write down your header between these. the `1` which is inside The header tags represent degree of the heading character size. There are 6 size header you can type on HTML.

####B. Add a Link 

When you steer user another page of your webpage or anther webpage you should add link on your page but how? On HTML you should Write down like this: `<a href= "http://your website domain">your Link tag</a>`.

####C. Add an image
We use an image tag, like so: `<img>`. This tag is a bit different from the others. Instead of putting the content between the tags, you tell the tag where to get the picture using src. It's also different because there is no ending tag. It has` / `in the tag to close it: `<img src="url" />`.

##### Make link inside the images

Good work! Now you know how to add links and images to your website. Why not make that image a link? For example;

    <a href="http://www.codecademy.com/">
    	<img src="https://s3.amazonaws.com/codecademy-blog/assets/f3a16fb6.jpg"/>
    </a>

First we open our `<a>` tag and point the href to http://www.codecademy.com/ again.
But this time, instead of using text inside the `<a>` tag, we use an `<img>` tag.
Finally, we have our closing `</a>` tag.
Now when you click on the yellow duck, you will be taken to` http://www.codecademy.com`!

Placing one HTML tag inside of another is called nesting.