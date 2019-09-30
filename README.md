# Availity Homework Assignment

We highly recommend that you use one of the free source code management platforms (GitHub, GitLab or BitBucket) when storing your code.  Once you are ready for us to look at your answers, send us the link to your code.  If you have any questions about the homework, please do not hesitate to ask.

1. Tell me about your proudest professional achievement.  It can be a personal or school project.  	

In 2014, I participated in a Game Jam where my team of 5 people created an adventure/puzzle game called Shinobi Inu. In 48 hours, we learned the Unity game engine, then made a functional demo. Even though we were unable to fulfill our vision due to time constraints, the experience was invaluable both as a learning opportunity and as a chance to make something cool. 


2. Tell me about a book, blog, article or GitHub repo you read or liked recently, and why you like it and why you should recommend I do the same. 

I picked up “7 Habits of Highly Effective People” by Stephen Covey at the recommendation of one of the podcasts I listen to. Overall, I agree with the podcast’s review: that while the methodology laid out in the book was useful, the examples and applications are pretty dated. Since then, I have become much more rigorous in paying attention to the way I use my time, and keep a personal notebook to track my time and my activities.


3. If you were to describe to a 7-year old what Availity does, what would you say? 

Availity makes software that makes it easier for people going to the doctor to pay their doctor. 
	
4. Coding exercise: You are tasked to write a checker that validates the parentheses of a LISP code.  Write a program (in Java or JavaScript) which takes in a string as an input and returns true if all the parentheses in the string are properly closed and nested.

```js
function lispValidator(str) {
	var stack = [];
	for (let i = 0; i < str.length; i++) {
		if(str.charAt(i)=='('){
			stack.push('(');
		}
		else if (str.charAt(i)==')') {
			if (stack[stack.length-1]=='(') {
				stack.pop(); // matches an open parens
			} else {
				return false; // 
			}
		}
	}
	return stack.length == 0;
}

console.log(lispValidator("(())"));
```

5. Coding exercise:   For frontend engineer: Healthcare providers request to be part of the Availity system.  Using React framework, create a registration user interface so healthcare providers can electronically join Availity.  The following data points should be collected:

- First and Last Name
- NPI number
- Business Address
- Telephone Number
- Email address


