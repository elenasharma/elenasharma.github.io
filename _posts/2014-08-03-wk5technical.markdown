---
layout: post
title: "in a class of its own"
date:   2014-06-25 11:39:00
---
<h3><i>Ruby classes: the when, why, and how of them</i></h3>
<p>As an object-oriented language, Ruby views everything, even strings, booleans, and integers, as objects - and every object belongs to a class. So <i>when</i> do we use classes in Ruby? Well, all the time!</p>
<p>If you want to look up the behavior of one of the aforementioned objects, like a string or integer, you can go to the Ruby docs where all the built-in methods are listed under Class: Integer, for example. A class gives form to an object as well as describing what that object is able to do (in other words, its functionalities).</p>
<p>So <i>why</i> do we use classes? Well as we can see, by combining data and functionality classes consolidate information about objects neatly, accomplishing two tasks in one, which is pretty handy. Not only that, but if we want to use Ruby which, as I've said, is an object-oriented language, we can't really avoid using classes - there's no way to! So in order to not be an embarrassment of a Rubyist, it's important to learn <i>how</i> to use classes.</p>
<p>Let's model something simple: <b>making a sandwich</b>! Say you work at a sandwich 
cafe that has the rule that only one type of sandwich can be made each day. Each morning, a box of bread, with the number of slices written on the outside, arrives. You have a list of the possible sandwich types for that day, but you're not sure which one will be selected until the Chief Sandwich Maker arrives (sadly, not you). If you want to find out 
how many sandwiches you can make and predict the possible sandwiches for the day, you could write a Sandwiches class with variables and methods for the task!</p>
	<img src="http://i1060.photobucket.com/albums/t460/Elena_Sharma/ScreenShot2014-07-06at105201PM_zps19999839.png">
<p>In this code, you can clearly see that the class in question is called 
Sandwiches - and there's a lot of stuff inside that class! Starting at the top, the first method <b>initialize</b> is a method that creates new instances of the classes; in other words, when you run <b>class.new(some_input, some_other_input)</b>, you will have created a new instance of that class with an object created with some_input and some_other_input.</p>
<p>Initialize also records <b><i>instance variables</i></b>, which here are <b>@slices</b> and <b>@types</b>. Instance variables can be used by all the methods in a class because again, they are part of the same instance - the created object. Still unsure about instances? Maybe this will help:</p>
<img src="http://i1060.photobucket.com/albums/t460/Elena_Sharma/ScreenShot2014-07-06at110828PM_zps201ad670.png">
<p>Here, two different instances have been created: <b></i>test1</i></b> and <b><i>test2</i></b>, which have entirely different inputs. Both objects are initialized by being assigned to the result of Sandwiches.new (which is calling the class initiator) and passing in the two inputs for that instance. These inputs, assigned to instance variables in <b>initialize</b>, can also be seen in <b>num_sandwiches</b> and <b>make_sandwiches</b>. So instance methods can be used across methods in the same class!</p>
<img src="http://i1060.photobucket.com/albums/t460/Elena_Sharma/a6197eb2-0e55-41ee-af80-f72a313893b1_zpsa4002560.png">
<img src="http://i1060.photobucket.com/albums/t460/Elena_Sharma/749441ef-c9d7-43f7-aeac-23a50ccd8e94_zpseda4be82.png">
<p><small>(here are two possible outputs of calling the instance methods on these two objects - notice that the types of sandwiches change due to the use of .sample!)</small></p>
<p>Now we know that everything in Ruby is an object and every object belongs to a class, which can contain data and detail behavior. In the class I created, it held data to be defined by instances and the functionalities of outputting the number of sandwiches that could be made and a possible day of sandwich-making, given the number of slices and sandwich options. We also saw that instance variables can be used across methods, which is extremely useful. So when you're making objects, which you'll definitely be doing if you pursue becoming a Rubyist, make sure to keep it classy!</p>
<p><small>(I'm sorry, the class puns are just begging to happen.)</small></p>