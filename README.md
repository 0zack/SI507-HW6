# JavaScript assignment

### Names of people you have worked with on this assignment
* **Yeongjae (Zack) Lim (zacklim)**

## Questions & code instructions

* **What does a code comment look like in JavaScript? What character/s do you have to put before a comment?**

//comments

* **Explain what needs to happen to get a JavaScript program to "run", given the JavaScript you've seen in this assignment.**

You should use '<script type="text/javascript">' before starting programming JavaScript.

* **What functions in JavaScript seem to be similar in function to the `print` function in Python? (There are two.) Why might you use one and not the other? Explain briefly.**
Two ways which are similar to the Python function 'print' are:
```js
alert();
console.log();
```
I would use the first one because it is the direct way to show what I want to print. 

* **What code would have to comment out to get rid of the pop-up box when you load the page? (Related to the last question.) Do that in the code file, and then, add code so that a text box will appear that contains the current date and time! *HINT:* Look through the rest of the code first...**

I would comment out 'alert()' function to get rid of the pop-up box.

* **How can you put your own name at the top where it currently says "A name"? Explain very briefly how to do so, and replace `A name` in the web page with your own name.**

I will change a code like below:
```js
document.querySelector('h1').innerHTML = "Zack";
```
* **What does the word `document` represent in this code? Explain briefly.**

The word 'document' represent the whole code in the current html file.

* **What is happening in line 12 ( 
		`document.querySelector('#items').innerHTML = document.getElementsByTagName('li').length`
)? Explain, briefly (<= 2 sentences).**

`document.getElementsByTagName('li').length`
finds the number of elements with the tag name 'li' and give the number to the element with the id 'items'. In this page, since the the elements of 'li' is 9, and the element with the id 'items' is <span> element, the text in the text box becomes 
`The number of list items for this page: 9`

* **What color would the background of this page be <u>if there were no JavaScript in this page</u>?**

The color of the background will become white which is the default color.

* **Why are there a couple of gray boxes on the screen with a different colored border? How could you edit this code to make them a different color? Explain briefly. Then edit the code to make those boxes some shade of blue, of your choosing.**

You can easily change the border color in CSS part.
```css
p{border: 3px solid #fe0000;}
```

* **Edit the code so that, if you highlight `McGill University` and copy it, you see the text `O Canada` near the bottom of the page. Briefly explain why you made the edits that you did -- how did you know/figure out what to do?**

* **In the original code, when you click the button that says `Wow`, you see a text box! Wow. Explain briefly in your own words why the following code causes that to happen:**

```js
function handleClick(){
	alert("hello");
}
```
**and**

```js
<button onclick=handleClick() id="wow-button">Wow</button>
```
Since the function 'handleClick()' has already been defined to show the pop-up text box in the JavaScript part, and the button element in HTML has onclick parameter for the function which works when the button is clicked.


* **Knowing what you learned from the previous question, add code/markup to the `jsPracticeLab.html` file *so that* there is a button with the text `Spring Equinox 2019` on it somewhere on the page, and when that button is clicked, a text box containing the text `March 20, 2019` appears. (There's no function -- that I am aware of -- to automatically get this info, you've got to type it yourself.)**

I revised that by following code:
```js
function new_btn(){
		alert("March 20, 2019");
}
```
```html
<button onclick=new_btn() id="new-button" style="width: 500px; height: 80px; font-size: 25px; color: #fff; background: #282828; border-radius: 10px;">Spring Equinox 2019</button>
```


### The next few questions address the `jquerylib_submit_example.html` file.

* **Check out the file `jquerylib_submit_example.html`. This is an example of code that uses a package called `jQuery` (and this will need you to have an internet connection to run it properly, although the other file does not). Check out resources above for more on jQuery!**

* **When you enter input that isn't valid, you see an error that is red. Why is the error in red? Why is the response for valid inputs blue?**

If the input is valid, the text is displayed with the class name good which its color is blue, and otherwise it is shown with the class name error which its color is red.

* **What is this line `var regex = /^[a-zA-Z]+$/;` helping with? And if you googled something to figure that out, what did you google, and what, briefly, did you learn? (If you didn't need to google, you can leave that out, but explain briefly what that line is helping the program do, anyway.)**

Regex means a regular expression. It is used when you need to find some words, phrases, or sentences that match some conditions. For instance, a-z matches a character in the range "a" to "Z".

* **What's different about the syntax of conditional statements in JavaScript, compared to Python?**

In a conditional statement, JavaScript uses parentheses to separate the execution statements, whereas Python uses clone (':') and indent.

* **What do you think the `10000` refers to in the code `.fadeOut(10000)`?**

It means the duration of fade out. 1000 means a second, so 10000 means 10 seconds.

* **What do you think is going on with the following code at the beginning of the program? Note that the most important thing to do for answering this question is to be thoughtful and clear, not to be absolutely correct:**

```js
$(document).ready(function(){
    $("form").submit(function(event){
```
`$("form").submit(function(event){` is a function definition when the form is submitted with the element `<input type="submit" value="Submit">`. And `$(document).ready(function(){` is to make the rest codes in its parentheses works when the document is loaded entirely.

* **Add some code to the `jquerylib_submit_example.html` file so that, if the input is valid and is specifically the text `hello`, rather than the visible output being `Nice!` in blue, the visible output should be `Hello to you too!`, also in blue, just like `Nice!` is.**
	* *HINT:* You'll have to make some changes to the conditional statement, and possibly look up some JavaScript conditional syntax. You'll also need to look carefully at what generates visible output right now.

I did.