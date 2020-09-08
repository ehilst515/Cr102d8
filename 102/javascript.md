# JavaScript
We previously learned that HTML provides the framework of a website, and using CSS provides the ability to change how a website is presented. The final piece of the website puzzle is **JavaScript**, which is a language commonly used to make things that can be interacted with and that can change the way a webpage behaves. For example, the JavaScript code below can greet a visitor different ways depending on the time of day:

```
var today = new Date();
var hourNow = today.getHours();
var greeting;

if (hourNow > 18) {
    greeting = 'Good evening!';
}   else if (hourNow > 12){
    greeting = 'Good afternoon!';
}   else if (hourNow > 0) {
    greeting = 'Good morning!';
}   else {
    greeting = 'Welcome!';
}

document.write('<h3>' + greeting + '</h3>');

```

A .js file can be made and used as the source within an HTML file using:

```
<script src="(directorylocation/filename.js)"></script>
```

Correctly placing this code will make the properly timed greeting work! 

*Note that JavaScript is written with `OBJECT.METHOD`. Each `OBJECT` has certain **members** it can access, and the period between the `OBJECT` and `METHOD` is called "member operator".*