---
layout: post
title: "SQL injection attacks!"
date:   2014-07-20 13:36:00
---

<h3>What is SQL?</h3>
<p>So you're a new developer and you're just getting to know Structured Query Language or SQL, as it's known. SQL is a handy language that interacts with database systems - operates and queries them, mostly - that form the functionality of many web applications. Simply put, SQL can create schemas and update/insert/delete/query data - it manages data in database systems. Sounds useful, right?</p>
<h3>SQL injection</h3>
<p>But there's a well-known issue - <a class="postlink" href="https://www.owasp.org/index.php/Top_10_2013-T10">considered the foremost threat to web applications</a> - with SQL called an <b><i>SQL injection attack</i></b>. It's a type of security attack that can bypass the application's structure to retrieve information from the database, bypass authentication measures, or alter the content of the database.</p>
<h3>How to combat it</h3>
<p>Never fear, there are ways to fight back against SQL injection attacks! The coder needs to make sure to correctly filter user input for escape characters. In addition, all user-supplied fields should be strongly typed - so that if a piece of input is supposed to be an integer, the programmer needs to put checks in place that make sure that the input is in fact an integer. In essence, SQL injection attacks stem from a security flaw in the code of a web application. So whichever system or language is being used, the programmer needs to make sure that user input is strongly typed properly filtered.</p>
<h3>SQL vs. NoSQL</h3>
<p>Let's be honest, I'm a total beginner programmer. So my understanding of the difference between these two types of databases is that SQL is a relational database - storing relations of fields, often working in a more table-like or tabular structure - and NoSQL (or, Not Only SQL) is non-relational, using a simpler, sometimes considered sleeker interface. SQL seems to have more standardized interfaces and more clear-cut relational structures, though some operations might be slower than in NoSQL, which grants the user more control over how s/he will access information, but lacks a standard interface. Beyond that broad overview of the two languages, a lot of the information is over my head. I'm glad we learned about SQL first, definitely - the tabular nature is a nice, straightforward structure for us beginners. But I'm interested to see what kind of alternatives NoSQL presents, since I can't imagine something <i>non</i>-tabular really.</p>
<h3>optimizing SQL queries</h3>
<p>As far as optimizing SQL, which is considered by some to be clunkier than NoSQL? We can avoid using wildcards - '%' - and instead use 'whatever%', which does not slow down the database as much. It is also easier and faster for SQL to find data based on a positive match than a negation through operations like NOT, NOT LIKE, NOT IN, etc. We should also use LIMIT to limit the resulting data from a query. <a class="postlink" href="http://hungred.com/useful-information/ways-optimize-sql-queries/">this site</a> contains more examples of how to optimize SQL queries, especially if they were being run on a giant database.</p>
<h3>in conclusion...</h3>
<p>Clearly, there is a LOT of information out there about SQL and other types of database languages - their weaknesses, strengths, optimization strategies, and much more. I'm looking forward to continuing to learn more about these languages and how to navigate them without exposing my web applications to injection attacks!
</p>