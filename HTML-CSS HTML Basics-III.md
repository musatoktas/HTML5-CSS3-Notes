# HTML BASICS III #

----------

In this page we will cover some important part of HTML. Such as;`<table>`s, `<div>`s, and, `<span>`s. 

## Table's
 Let's learn more about HTML. Tables mean what you prepare in excel. They are include datas about some topics (it can be about everythink you want). Now we will do them on HTML. To create table first of all you should know how many pixels the border thickness and add inside these tags `<table border="1px">-</table>` inside body part of HTML page. For example

	<body>
		<table border="1px">
			<tr><!-- Each row you should write this <tr>-</tr> -->
				<td><!-- Each content cells you should write this <td>-</td> -->
					First Content
 				</td>
			</tr>
		</table>
	</body>

####1. Adding header to our table
We are preapring table for what? We have to indicate that on top of our table. Tables occuring by two parts like HTML page, and human body. First head, and Second Body. Head tags are; `<thead>-</thead>`, Body tags are; `<tbody>-</tbody>`.
<body>
      
        <table border="1px">
            <thead>
                <tr>
                    <th>
                     Famous Monster
                    </th>
                    <th>
                     Birth Year
                    </th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>King Kong</td>
                    <td>1933</td> 
                </tr>
                
                <tr>
                    <td>Dracula</td>
                    <td>1897</td>
                </tr>
                
                <tr>
                    <td>Bride of Frankenstein</td>
                    <td>1935</td>
                </tr>
            </tbody>
        </table>
        
    </body>


It will appear on editor like this:
<body>
  
<table border="1px">
<thead>
<tr>
<th>
 Famous Monster
</th>
<th>
 Birth Year
</th>
</tr>
</thead>
<tbody>
<tr>
<td>King Kong</td>
<td>1933</td> 
</tr>

<tr>
<td>Dracula</td>
<td>1897</td>
</tr>

<tr>
<td>Bride of Frankenstein</td>
<td>1935</td>
</tr>
</tbody>
</table>

</body>

####2. Adding title to our table
Our table is missing a title. We want to add a title row that goes all the way across the top. Its in the head part of table. I mean inside here;`<thead>-</thead>`, an dit must be different row. Let me show on an example.

    <thead>
                <tr>
                    <th colspan="2">Famous Monsters by Birth Year</th>
                </tr>
                <tr>
                    <th>Famous Monster</th>
                    <th>Birth Year</th>
                </tr>
            </thead>

To do so, we need to use the `colspan` attribute for the `<th>` tag. By default, table cells take up 1 column. If we want a table cell to take up the space of 3 columns instead of 1, we can set the `colspan` attribute to 3.

It looks like this:

<body>

<table border="1px">
<thead>
<tr>
<th colspan="2">Famous Monsters by Birth Year</th>
</tr>
<tr>
<th>Famous Monster</th>
<th>Birth Year</th>
</tr>
</thead>
<tbody>
<tr>
<td>King Kong</td>
<td>1933</td> 
</tr>

<tr>
<td>Dracula</td>
<td>1897</td>
</tr>

<tr>
<td>Bride of Frankenstein</td>
<td>1935</td>
</tr>
</tbody>
</table>

</body>

You can change size font color or font typ by using style attribute as you can know. Here is a bit of example.

    <tr>
    	<th colspan="2" style="color: red; font-size: 19 px; font-family: Times New Roman">Famous Monsters by Birth Year </th>
    </tr>
    
It will appear like this;

   <tr>
	<th colspan="2" style="color: red; font-size: 19 px; font-family: times new Roman">Famous Monsters by Birth Year </th>
</tr>
    
  
##Divide "`<div>-</div>`"

----------
There is a one of the useful tags of HTML. Its working for dividing your editor to parts.For examle You want a litlle part of your page yellow. You can do it by using this tags. You can also add link on it, you can texting on it etc. Here is an example of it:

    	<body>
		<div style="width:50px; height:50px; background-color:red"></div>
		<div style="width:50px; height:50px; background-color:blue"></div>
		<div style="width:50px; height:50px; background-color:green"></div>
		<div style="width:50px; height:50px; background-color: yellow"></div>
		</body>

It Will appear like this:
	<body>
		<div style="width:50px; height:50px; background-color:red"></div>
		<div style="width:50px; height:50px; background-color:blue"></div>
		<div style="width:50px; height:50px; background-color:green"></div>
		<div style="width:50px; height:50px; background-color: yellow"></div>
		</body>

You can also add Link on it by using `<a href="link">-</a>` tags. here is an example of it.
	

	`<a href="http://www.codeacademy.com"><div style="width:50px; height:50px; background-color:yellow"></div></a>`
You can try it by clicking yellow area:
<body>
		<a href="http://www.codeacademy.com"><div style="width:50px; height:50px; background-color:yellow"></div></a>
</body> 
Note: Next Lesson We will focusing more one `<div>-</div>` tags.

##Span Tags

It will work for manage the small part our pages like some of the words. For example you always want to emphasise one word. You can do that by using this tags. Here is an example:

    <p>This text is black, except for the word <span style="color:red">red!</span></p>
	

# Summary 

----------

----------
Woosh! We've learned quite a bit.

What can you do now?



- Write an HTML comment
- Create a list (ordered and unordered)
- Make text stand out using `<em>` and `<strong>`
- Change the color, size, and alignment of text using the style attribute
- Create HTML tables

Also;
Divide up your webpage for easy styling with `<div> `tags
Select pieces of text and change their properties using `<span>` tags
In the next course, we'll see how we can take much of the styling we've been doing—such as controlling font family, font color, and text alignment—and put it in its own separate file. By doing that, we can use tags like `<div>` and `<span>` to impart style to our pages without writing style="color:red" every single time!

See you on the next page!!



