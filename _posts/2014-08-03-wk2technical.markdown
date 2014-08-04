---
layout: post
title: "displaying inline vs. inline-blocks"
date:   2014-06-10 14:47:00
---
<p>So this week, I'm going to explore some methods of displaying HTML elements - or a couple of different ways of telling things to appear. It's hard, especially when they sound so alike, but there is definitely a difference between <span class="thesis">displaying elements as inline versus displaying them as inline blocks</span>.</p>
<p>The first thing to ask here is, what do we mean by <i>display?</i>  A CSS property, display's settings specify the type of box that will be used for an HTML element. The default setting is inline, which is how the text inside this current paragraph element looks right now, as you are reading it - the words are <i>in line</i> with each other.</p>
<p>Interestingly, the default setting for paragraphs are actually not inline, but as block elements. A <b>block element</b> has width and height that can be defined and each block element starts a new row. The default settings of two paragraphs can be seen here:</p>
<img src="http://i1060.photobucket.com/albums/t460/Elena_Sharma/image_ex1_zpsb83c95e8.png">
<img src="http://i1060.photobucket.com/albums/t460/Elena_Sharma/code_ex1_zps004f8a91.png">
<p>The code for these two paragraphs can also be seen above. As you can see, there are two paragraphs which, as we might expect now knowing how blocks behave, are on separate rows.</p>
<p>So what would displaying inline or displaying as inline-blocks do? Well let's take a look. Displaying <b>inline</b> with these two paragraphs results in this:</p>
<img src="http://i1060.photobucket.com/albums/t460/Elena_Sharma/image_ex2_zpsd2a544bb.png">
<img src="http://i1060.photobucket.com/albums/t460/Elena_Sharma/code_ex2_zpsf9325907.png">
<p>We see here that telling these two paragraph elements to display inline actually results in all of their text running together - in lines! But what if, rather than having each <i>word</i> side-by-side, but we wanted to think bigger? What if we wanted the two paragraphs themselves to be side-by-side, in line?</p>
<p>That's where we get to the concept of the <b>inline-block</b>. <a class="postlink" href="http://robertnyman.com/2010/02/24/css-display-inline-block-why-it-rocks-and-why-it-sucks/">Robert Nyman</a> defines the inline-block thus:</p>
<p class="quotation">Basically, it’s a way to make elements inline, but preserving their block capabilities such as setting width and height, top and bottom margins and paddings etc.</p>
<p>I'll change my code to display inline-block instead of just inline and I'll see what I get. Theoretically, I should have two blocks side-by-side in the same line, preserving their block capabilities.</p>
<img src="http://i1060.photobucket.com/albums/t460/Elena_Sharma/img_ex3_zps836a1d3b.png">
<img src="http://i1060.photobucket.com/albums/t460/Elena_Sharma/code_ex3_zpsc4b93c12.png">
<p>Awesome! (Note that in order for the blocks to be side-by-side, the body width of 500px had to be removed since that was too narrow a container for two 300px-wide blocks to be side-by-side in) Just to test if the block capabilities (like width and height) are <i>really</i> preserved, let's set the two blocks to different widths, the yellow to 100px and the red to 400px wide.</p>
<img src="http://i1060.photobucket.com/albums/t460/Elena_Sharma/img_ex4_zps73d3fd57.png">
<img src="http://i1060.photobucket.com/albums/t460/Elena_Sharma/code_ex4_zps9ef94ad3.png">
<p>Great! One final thing to note is that no matter the heights of these blocks, they are <i>inline</i> with respect to the bottom of their blocks. So in conclusion, we see that <b>inline</b> means for the text itself to be inline, but <b>inline-block</b> as a display value preserves the block-ness of an element, such as its width and height, as well as top and bottom margins and padding. Inline-blocks are considered an alternative to using float to arrange two elements side by side (since float has a number of strange behaviors like collapsing parent elements, among others), but so does inline-block, like being dependent upon white space in HTML - so make sure to find out those behaviors when you're deciding which of these methods to use!
</p>