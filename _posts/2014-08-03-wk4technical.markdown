---
layout: post
title: "getting loopy with Ruby"
date:   2014-06-26 14:05:00
---
<p>Learning how to loop in a programming language is a must for any developer because loops are so powerful - they apply some method or block  of code a specified number of times, allowing for counting through sets of information, for instance.</p>
<p>The main Ruby loop methods are <b>while</b>, <b>for</b>, and <b>until</b>.</p>
<p><b><i>while</i></b> loops, such as </p>
<p class="postcode">while (x == y) do<br>
	puts 'x is still equal to y'<br>
	end
</p>
<p>carry out the action (here, the 'puts') as long as the condition (here, 'x != y') is true.</p>
<p><b><i>for</i></b> loops, like</p>
<p class="postcode">for i in 0..10<br>
	puts i<br>
	end
</p>
<p>are given a set range (here, the range from 0 to 10) that determines the number of times the code (here, 'puts i') will be executed.</p>
<p><b><i>until</i></b> loops, like this example,</p>
<p class="postcode">until (x == y) do<br>
	puts 'x is still NOT equal to y'<br>
	end
</p>
<p>are somewhat like while loops except instead of executing as long as the condition is true, until loops execute as long as the conditional (here 'x == y') is <i>false</i>.</p>
<p>There are also other looping methods, such as <b>.times</b> and <b>.each</b> - code like</p>
<p class="postcode">3.times do</p> 
<p>will, as it might seem it should, execute whatever it's doing 3 times, while</p>
<p class="postcode">(somearray).each do |n|</p>
<p>will execute its code for each of the members of the input, which can be any kind of list of variables.</p>
<p>So how should you choose between all these types of loops? It can seem a little overwhelming, but it helps to think through how you want to use the loops in simple terms. Say you have a list of 10 items and you want to do something to all of those items. Using <b>.each</b> would be the best option here. But what if you wanted to use only half of those? Then you might want to say '5.times do' (your code).</p>
<p>When it comes to <b>for</b>, <b>while</b>, and <b>until</b>, let's think of some other examples. Say you have a program that outputs grades, given a list of student grades in increasing order, but you only want to output the grades that are below 70 (so you can send them to the students or parents). In this case, you could use 'until grade == 70' OR 'while grade != 70'. Until and while should be used in cases where you have some sort of cutoff for your range and they can be used pretty interchangeably, in my opinion, depending on if you like defining things by what they are or what they are NOT.</p>
<p>As for <b>for</b>, let's say again that we have a set of student grades in increasing order and that we have a function that is supposed to output the middle 50% (and we know the number of grades we have, like 20). For can get at specific ranges within a list, so think 'for i in 5..15'.</p>
<p>Hopefully this was a helpful introduction to some of the looping methods in Ruby! I'm still trying to figure out when to use these myself, but I think it's fairly straightforward if you write good pseudocode and really ask yourself: am I trying to do this x number of TIMES? Do I want to do this to EACH item in a list? Do I want to do something UNTIL a certain point or WHILE some condition is true? Or do I want to do something FOR a specific range of items? (okay, that last bit was cheesy, but again, hopefully good summary).</p>
<p>Happy looping, everyone!</p>