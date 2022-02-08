# Strings

In this tutorial, you're going to learn more about Python strings.
So I've defined this course variable and set it to Python for beginners:
````python
course = 'Python for Beginners'
````
now earlier I told you could use both single and double quotes to define a string, but there are times you have to use a specific form, otherwise you're going to run into issues. 

Here's an example: imagine you wanted to change this string into _Python's course for Beginners_.
So we want to add an apostrophe, lke this:
````python
course = 'Python's course for Beginners'
````
You can immediately say this is going crazy, because our string starts in 'P' and then terminates in 'n'.
All these characters that we have here after the second apostrophe (_s course for Beginners_), Python interpreter doesn't know what they are. 
So, to solve this problem, we need to use double quotes to define our string, so we can have a single quote in the middle of the string.
So, let's change this to double quotes, now you can see it adds another double quote to close it.
You have to manually remove this, and also one more time at the beginning of the string, we need to add another double quote.
````python
course = "Python's course for Beginners"
````
Now you can see error is gone, so if you print _course_
````python
print(course) 
````
we see _Python's course for Beginners_.

Now let's say we don't want this apostrophe here, so we have _"Python for Begginers"_, but we want to put _Beginners_ in double quotes.
Once again, if you add a double quote here, Python interpreter gets confused because it assumes the second double quote indicates that end of the string, so it doesn't know what these characters are:
````python
course = "Python for "Beginners"
print(course) 
````
So, to solve this, we need to change our double quotes to single quotes, and then we can add double quotes in the middle of the string:
````python
course = 'Python for "Beginners"'
print(course) 
````
So there are the cases for using single or double quotes. Now, in all the examples, I've shown you so far we only deal with short strings, but what if you wanted to define a string that is multiple lenghts?
For example, what if you wanted to define a string for the message that we send in an email.
In that case, we need to use triple quotes. So, we have 3 quotes to start out our string and 3 quotes to terminate it. Again, these quotes can be single or double quotes.
Now, with this we can define a string that spans multiple lines. For example, we can say _Hi Teresa, Here is our first email to you. Thank you, Patrick_:
````python
course = '''
Hi Teresa, 

Here is our first email to you. 

Thank you, 

Patrick
'''
print(course) 
````
So, we get this beautiful multi-line string.
Now, let's change this back to something simple, so, we can look at other characteristics of strings in Python.
I'm going to use single quotes and set the course name to _Python for Beginners_. 
Now here we're going to use square brackets to get a character and a given index in this string.
So, to get the first character we use square brackets and type _0_:
````python
course = 'Python for Beginners'
print(course[0])
````
So the index of the first character in this string is _0_. 
In other words, this is how Python strings are indexed: _0, 1, 2, 3_, etc 
So, the index of the first character is _0_, the index of the second is _1_, and so on.
So, if we run this program, we get _p_. We can also use a negative index here.
And this is one of the features that we don't have in other programming languages as far as I know.
So we have negative index, we can get the characters started from the end.
So if I pass negative 1 here, assuming that _0_ is the first character, negative 1 is the last character.
So, when we run this program we shoul see _s_:
````python
course = 'Python for Beginners'
print(course[-1])
````
If we pass negative 2, this will return the second character from the end (_r_).
Okay? So, please pay close attention to this square brackets syntax, because quite often it's the topic for online Python tests or university exams.
We can also use a similar sintax to extract a few characters instead of one character.
For example, if we type:
````python
course = 'Python for Beginners'
print(course[0:3])
````
Python interpreter will return all the characters starting with _0_ all the way to _3_, but it does not return the character at the index _3_.
Now here we also have default values for the start and end index. 
So, if we don't supply the end index, Python will return all the characters to the end of the string:
````python
course = 'Python for Beginners'
print(course[0:])
````
But if you change the start index to _1_, this will exclude the first character:
````python
course = 'Python for Beginners'
print(course[1:])
````
Similarly, we have a default value for the start index. So, if we don't supply it, and add and end index like _5_, Python will assume _0_ as the start index: 
````python
course = 'Python for Beginners'
print(course[:5])
````
Now what if we leave both the start and the end index? 
In this case _0_ will be assumed as the start index and the lenght of the string will be assumed as the end index.
So with this syntax, you can basically copy or clone a string:
````python
course = 'Python for Beginners'
print(course[:])
````
In other words, if I define another variable here, let's call it _another_ and set it like this:
````python
course = 'Python for Beginners'
another = course [:]
print(another)
````
The second variable will be the copy of the first.
Now here's a little exercise for you:
Define a variable, called _name_, and set it to _Jane_.
When we print:
````python
course = 'Jane'
print(course[1:-1])
````
What do you think we're going to see on the terminal?

# Formatted Strings

# String Methods