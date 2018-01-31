---
title: "Non Verbal Communicator<br>
Feature 1 Unit Testing"
image: img/placeimg_900_300_tech.jpg
lead: "Unit Testing of Feature 1"
---
<p>
<b>Feature</b><br>
<li>The system must be able create and retrieve a PEC Object.</li>
</p>

{% include unit-testing.html %}

<p>
<b>Requirement</b><br>
<li>The system must have a way to represent Picture Exchange Communicator Object</li>
<li>The system must have way to cache PEC's</li>
</p>


<p>
<b>UML class diagrams</b>
</p>
<img src="img/nvc/Feature_1_Design.png">

<h2>Testing Evaluation</h2>
I spent the last few days following the tdd process. I felt very accomplished when<br>
I was able to create failing tests for my proxy dao. I didn't implement the uut<br>
classes but I was able to construct mocks of the proxy's host, which was also not implemented.<br>
I felt reassured when I implemented the proxy and the verify then return methods were causing my tests to pass.<br>
Next up was the actual PecSQLiteDAO Which I intended to be a singleton.<br>
I ran into issues with my PecSQLiteDAO and DB integrated test. I ended wiping out the apps actually DB<br>
instead of using a test DB. After I began hacking and adding extra constructors<br>
and using in memory cache and a new DB table name my integrated tests worked <br>
in isolations from the apps production code. I felt accomplished when I closed my<br>
laptop and went to bed. However as I laid in bed the inner programmer in my head<br>
sat at his laptop reviewing the work I did. I typically try to keep my code as clean<br>
as I can but everything I did smelt wrong. I'm realizing that I may have incurred<br>
some technical debt. I'm going to halt my project to gain some more knowledge on<br>
dependency injection. I think dagger is the best route to go so hopfully the second post of my testing<br>
reveals how I refactored my horrendous code failure.
