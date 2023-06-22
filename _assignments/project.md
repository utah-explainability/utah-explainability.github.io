---
title: Project
include_nav_home: false
---

# Project

* [Overview](https://utah-data-mining-spring23.github.io/assignments/project/#overview)
* [Project Proposal (5 points)](https://utah-data-mining-spring23.github.io/assignments/project/#project-proposal-5-points)  
* [Data Collection Report (10 points)](https://utah-data-mining-spring23.github.io/assignments/project/#data-collection-report-10-points)      
* [Intermediate Report (15 points)](https://utah-data-mining-spring23.github.io/assignments/project/#intermediate-report-15-points)        
* [Final Report (50 points)](https://utah-data-mining-spring23.github.io/assignments/project/#final-report-50-points)         
* [Poster Presentation (20 points)](https://utah-data-mining-spring23.github.io/assignments/project/#poster-presentations-20-points)

## Overview 

Your project will consist of five elements.  

* Project Proposal: Due January 25
* Data Collection Report: Due February 15
* Intermediate Report: Due March 20
* Final Report: Due April 12
* Poster Outline: Due April 17
* Poster Final Version: Due April 20
* Poster Presentation: April 24 (3:30pm - 5:30pm or 6:00pm)

As in any research in order to get people to pay attention, you will need to be able to present your work efficiently in written and oral form.  

You may work in teams of 2 or 3, but the amount of work you perform will need to scale accordingly.  Teams of size 1 might be allowed under unusual circumstances with special permission from the instructor.  All students will need to have clearly defined roles as demonstrated in the final report and presentation.  I highly recommend groups of size 3.  Although the project work will scale with students, the administrative parts will remain constant, so having a large group will make it easier for you.  

Note that some topics will not be covered before many elements of the project are due.  I realize this is not ideal.  However, typically, most work on a project is crammed in the last week or two of the semester, which is also not ideal.  In the past this has lead to much stronger projects without considerably more work required.  


### Scale of Project

The specifics of the project will be very flexible.  I expect each student to perform data mining on some real data set.  The goal is to gain more in depth experience in some aspect of the class, and to do so in a setting where the instructor can provide guidance.  

The lectures will cover the material, the homeworks and quizzes will reinforce the material, and this project should provide deep understanding of some aspect of the material.  Students who demonstrate a deep understanding of some aspect of data mining covered in the class through their project will receive high grades.  

Project options may include:  

* apply advanced techniques from the class towards a real data set
* compare several basic techniques from the class towards a real data set
* propose and test extension to techniques from class on a real data set

### No double dipping projects across multiple classes
A
You can not submit the same project to this class and another class that you may be taking at the same time. If you are doing related projects in two different classes, there may be some overlap (e.g. in code libraries, etc.), but they should not be identical. A project that is found to be double-submitted will receive zero credit. If you have questions about this policy, please contact the instructor.

### Late project components

To get full credit for a project assignment, it must be turned in through Canvas by the due time. Different aspects of projects are due at different times, so please carefully review when each component is due. For PROJECT assignments, the same penalty as for homework is applied for **every component** of the project that is submitted late: Once the deadline is missed, those turned in late will lose 10%. Every subsequent 24 hours until it is turned another 10% is deducted. Assignments will not be accepted more than 48 hours late and will be given a 0. **You CANNOT be late with two project components _without penalty_.** Each team member gets deducted scores for late project components.  

All assignments, unless otherwise announced, must be submitted to the designated area of Canvas. **Do not submit assignments via email.**

### Grading 

If you believe there is an error in grading, you may request a regrading within one week of receiving your grade. Requests must be made by email to the instructor, explaining clearly why you think your solution is correct.

You can earn extra points with poster presentation. 

The class operates under the School of Computing’s [policies and guidelines](https://handbook.cs.utah.edu/2019-2020/Academics/policies.php). Among other things, we will adhere to the [academic misconduct policy](https://www.cs.utah.edu/docs/misc/cheating_policy.pdf). 


## Project Proposal (5 points)

**Due January 25** 

Prepare a **100 to 200 word** document outlining your plan.  This should contain:

* who is in your group
* what data you plan to use and where you plan to get it from
* what structure you want to mine from the data
* why this problem is interesting
* what is new, or what I (the instructor) will learn


The last bullet should try to make clear why this is **more** than just another homework assignment.  Either 
you are applying data mining techniques to a specific data set in a way it has not (to your knowledge) been done before;
you are comparing several techniques when you are not sure which is best, or what advantages each has;
you are proposing some new variation to some existing idea.  

It is not uncommon for the instructor will provide feedback and alter or modify your proposed plans.  This can either happen by students stopping by to discuss with the instructor or TA before the proposal is due, or will come in feedback on the specific proposal.  
This step is most important when the topic is related to material that is covered later in the class.  

To be clear, if there are multiple students on a project team, the project should scale accordingly.  This may for instance involve trying three extensions to a technique and comparing to see which works the best (for 3 students).  Or processing a data set in two phases using two consecutive techniques (for 2 students).  The work does not need to be split as such, but it should be clearly more than for a single student.  

If this is part of a larger project (e.g. part of your thesis work, extending your lab's work), please indicate its scope with respect to previous work.  

As an arbitrary way to separate this class from the Machine Learning class, we will **not allow projects with central focus on building a classifier**.  A classifier may be used to evaluate a result.    

### Topics  

The best projects occur on topics that students have experience with and/or are passionate about.  First look within your own experience, whether that is your research, your work, or your hobbies.   

If you still have trouble finding a topic, I suggest exploring these resources for interesting datasets to explore.  You cannot just explore a data set, you must propose to find some structure in it. 

* <https://www.kaggle.com/datasets>
* <http://snap.stanford.edu/data/>
* <http://www.census.gov/>
* <http://meta.wikimedia.org/wiki/Data_dumps>
* <http://storage.googleapis.com/books/ngrams/books/datasetsv2.html>
* <https://huggingface.co/datasets/allenai/c4>
* <http://kdd.ics.uci.edu/>
* <http://www.cise.ufl.edu/research/sparse/matrices/>
* <http://webscope.sandbox.yahoo.com/>
* <http://www.google.com/publicdata/directory>
* <https://aws.amazon.com/datasets>
* <https://dev.twitter.com/streaming/overview>
* <http://lib.stat.cmu.edu/datasets/>

If you have an advisor, they may also be good source of problems and data.  


## Data Collection Report (10 points)

**Due February 15**

Prepare an **at most 1 page** report describing what data you have collected (or for some larger settings like from Twitter) are continuing to collect.  

_Often a surprising amount of time in data mining is spent in acquiring and manipulating data.  And demonstrating a technique on a real data set can have dramatic impact in convincing someone of its usefulness._

Please report:
* How you obtained your data?
* How large is your data?
* In what format are you storing your data.  Describe the _abstract data type_, not just the file format.  
* Did you need to process the original data to get it into an easier, more compressed format (e.g., convert from one format to another one)?     

For this report, I really want you to focus on which of the abstract data types (e.g., matrix, graph, point set, set of sets, or a combination of these) that you will think of this data set as.  
In many cases you will not store the data in the original format, and you will need to convert it to another format.  I want you to think about this conversion along the idea of these abstract representations.  
This is usually the most challenging aspect for students.  These decisions should be discussed to answer steps 2 and 3 (above) fully.  

For instance, do not say data is a vector (which implies Euclidian distance) if the coordinates have different units, and are not compatible, unless the goal is only regression.  Do not have each entry be a piece of text; it can be a count of the number of a word or set of words, but not a piece of text.  This is usually not useful.  Same goes for a matrix representation with different meanings for each column.  Think carefully about this, and ask the instructor if you are not sure.  


## Intermediate Report (15 points)

**Due March 20**  at  **11:59 PM**.

_Each project team will be assigned 2 other project teams. **In class on March 22**, we will spend half the time with project teams meeting and peer evaluating each other's projects. Before March 22 class, you must read reports of two other projects. Teams will have an option to update their reports before evaluated by the instructor.  Remote students will be able to discuss over Zoom or other means if preferred._ 

Prepare an **at most 1 page per student** report describing your progress so far towards your proposed goal.  That is 2 students can turn in 2 pages, and 3 students can turn in 3 pages.  

Basically this intermediate report should demonstrate to the instructor that you have made non-trivial progress towards your goal.  

* For instance, perhaps you proposed to take a basic technique and slightly modify it.  Then this intermediate report should note that you have gotten the basic technique working.        

* Some basic plots or numbers from experiments that you ran (mainly to convince yourself) that shows everything is working can be included.            

* Perhaps you have finished all of the coding and setup already and just need to run experiments at this point.  Then note that and discuss what suite of experiments you plan to run for the final report.             


Specifically describe:

* What progress you have made towards your proposed goal? (just data collection is _not_ an option)
* If you tried some basic approaches: what worked well and what did not?
* What could be done to improve the basic approaches?
* What other experiments have you run and are you planning to run to demonstrate the effectiveness?


Updated reports: 

* Until Wed, March 22, 11:59 PM, you can notify the professor about whether you plan to update your report and how. 

* Professor will repond with a deadline for making updates.

## Final Report (50 points)

**Due April 12**

Your report will be **at most 4 pages per student**, single columned at 11 point or larger font. You can write a report as a group (up to 4*num_students pages) but it must be clear who did what. Margins should be at least 1 inch.  (If it is shorter, but contains all needed information, it will make the instructor happy.) 
However, you will be allowed an unlimited number of pages for references and appendices.  The report will be graded on the first four pages (per student), but additional information to support the first four pages may be appended and referred to.  The instructor will only read the appendix at her discretion.  Putting _all_ charts and figures in the appendix is not acceptable, and this will result in lost points.  

If you work in a group of more than 1 student, then it should be painfully clear what part of the project was worked on by each student.  If the distribution of work was complicated, a table in the appendix may be a good idea.  

**Why only 4 pages?**  A key aspect of scientific writing is efficiently conveying information.  I expect students to easily generate more than 4 pages of information, but you need to convey this information to me efficiently.  What are the key ideas?  What are the key experiments to show me plots for?  What is the relevant related work to highlight?  


### Content

* Provide a succinct title for your project (and your names!).  This is part of 4 pages/student.  Your poster must have the same title.  

* Explain the problem and motivation.  If you prepared a thorough proposal and intermediate report, then you may be able to borrow some material from there.  

* Explain what data you explored?  Where did it come from, how did you process it?  If you simulated to scale the experiments, how did this work?  
If your data collection report was thorough, you can likely reuse much of this material.  

* What is the **key idea** your project is built upon?  If there is no interesting ideas, I will be a little disappointed.  This should describe the rational behind and what you were hoping to discover about the different approaches you are comparing, or what extension you are proposing to a existing technique, or how you are applying a technique to a dataset where it has not been explored before.  

State this clearly in the beginning; try to make me excited to read the remainder of your report to find out how your idea played out!  

* Explain what you did.  Did you prove something?  Did you implement something?  Did you compare several things?  Did you extend something?  

* Explain what you learned.  This is often greatly aided through charts of experiments.  But you should also include what lessons you came away with in words; just charts or mathematics is insufficient.  


## Poster Presentations (20 points)

**Poster size MUST be 24 x 36 inches**

**Submit to Gradescope.**

**Presented April 24** at 3:00-5:30 or 6pm (in MEB hallway near SoC front office)

The class will have a poster session where each group will present their projects.  This will be open to a general audience.  Each group is responsible for one poster.  
Posters will be available by around 3pm in the MEB main office.  


### Content

I expect to see four things on your poster:

*  What is the problem and data you worked on?
*  What were the key ideas in your approach?  
*  What techniques from the class did you use?
*  What did you learn?

This is a great opportunity for the class to learn about a large variety of topics.  If you approach this poster presentation as a teaching experience, you will be more likely to succeed.  

There are two general types of posters:
  (A) ones that are meant to stand alone on a wall, with no interaction.
  (B) ones that are meant to serve as guides for a personal discussion on the topic.  
**Posters for the class should be type (B)**, since the main purpose will be a poster session with many people.  
As such, design your poster with this in mind:  Add any image that you would want to draw on the board or have on a slide if you are giving a presentation.  Posters with just text are typically not very useful.  All text should be large enough so that if you printed the entire poster on one piece of paper (standard notebook size) that it would be easy to read.  (Moreover, outlining a poster on a single piece of paper is an excellent way to start organizing your thoughts.)  
Make the posters eye-catching, so that people from a distance want to come over and find out more.  

**Illustrations, pictures, and examples are the key reason to make a poster.  Build your poster around these!**

For more recommendations on how to make a scientific poster, check out this tutorial: https://www.calliechappell.com/blog/scientific-poster.

_The department requests that you avoid full-color (e.g., black or blue) backgrounds with white text -- this makes the posters hard to print.  Some colors or using of fun design elements are great an encouraged, but if it does not make a difference, choose a white background._


### Making Posters

At the poster session there will be easels, foam boards,  and clips that can support posters.  I suggest two approaches to actually make the posters: 

**beginner / slides:**  Make 8 slides in PowerPoint (or equivalent) and post print-outs of the slides.  Make sure you use large enough font that it is easy to read.  The slides will help you structure your ``poster'' linearly to tell a story and help you modularize the presentation (both good things).  

**advanced / one-big-image:**  You can use applications like Powerpoint, Keynote, LucidChart, Omnigraffle, Illustrator, or IPE to create a single large slide.  
The pdf file should be called `firstname-lastname.pdf` (e.g., `ana-marasovic.pdf`; `firstname-lastname` replaced with one of the actual names of you group members) and the department will print it for you.  
If you make this to scale at 24 x 36 (either orientation), then the department will print it for you.  This should still have a clear title and narrative flow.  Other than including the key points, GO WILD, and do whatever you can imagine!  

**Your poster is not complete until it has been approved by me or TAs!**
Make sure the poster is in pdf format and is 24 x 36 feet, otherwise it will not be printed.  
Unless required for a special creative angle, the **background should be white**.  
Early submissions are greatly appreciated.  


### Poster Outline

A poster outline will need to be turned in (via Gradescope) **by April 17** at **5pm**.  This is to be the first full draft; but you can continue tweaking after this step.  Successful completion of this component is worth **5 points** towards the poster presentation.  Early submissions are much appreciated.  

You are also encouraged to stop by during office hours to discuss with the instructor or a TA.  
The outline should include a draft of the poster (either as a set of slides) or as a single document.  It should be near complete, so that the instructor/TA can make concrete suggestions to improve the poster.  


### Poster Session

Each student will be assigned two posters to write a small (250 words) summary on.  During the poster session each student will need to visit their assigned posters and learn about it enough to write the small summary.  

All students will vote one of their top 2 posters (judged by project accomplishments and quality of poster presentation).  They cannot vote for their own.  The top vote getter will earn a bonus 5 points, and the second top vote getter will earn a bonus 2 points.  
The past winners had very creative designs with lots of pictures or examples, _but still had all of the important points above_.

Also the instructor will visit each poster and ask for a **2 minute** overview of the project.  Prepare and practice this _short_ oral presentation.  
