---
layout: home
title: Local Explanations for Deep Learning Models
nav_exclude: true
toc: true
seo:
  type: Courses
  name: Local Explanations for Deep Learning Models
---

# {{ site.tagline }}
{: .no_toc .mb-2 }
{{ site.description }}
<br>
MoWe / 4:35PM-05:55PM	, [WEB 1230](https://map.utah.edu/index.html?code=WEB); in-person only
{: .fs-6 .fw-300 }

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign lead_ta = site.staffers | where: 'role', 'Lead TA' %}
{% for staffer in lead_ta %}
{{ staffer }}
{% endfor %}

{% assign teaching_assistants = site.staffers | where: 'role', 'TA' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}


Through **<span style="color: black;">this website</span>** we will share only the schedule and materials. Everything else---syllabus, announcements, discussion, turning in assignments/project components, communicating grades, policies---will be done through **<span style="color: black;">Canvas</span>**.

**What modalities does this course cover?** We will almost exclusively talk about **applications in NLP** and computer vision for **static images**. Inputs in these domains are represented with [embeddings](https://course18.fast.ai/lessonsml1/lesson11.html)---high-dimensional vectors of floating point numbers whose individual dimensions are not interpretable. If you are interested in applications that fall under data science, you will instead likely work with "meaningful" features such as income of a person or zip code of a certain location. This course is not about such applications. 

**What machine learning models this course covers?** We focus on deep learning models (deep neural networks) and we will almost solely talk about [transformer](http://jalammar.github.io/illustrated-transformer/)-based models.  

**Local vs. global explanations.** This course will **not** focus on [global methods](https://christophm.github.io/interpretable-ml-book/scope-of-interpretability.html) that analyze models'  behavior and internals such as [probing](https://nlp.stanford.edu/~johnhew/interpreting-probes.html). We focus on methods that answer questions such as: 

* Which part of the input led to assigning this label?             
* How to edit the input to change the answer to another?                           
* In plain English, why is this input assigned this label?                   
* Which training examples caused the prediction?   

**Pre-requisites.** This course doesn’t have formal pre-requisites because these days one can learn about machine learning and adjacent topics in many different ways, but we expected that you...

* ...are experienced with programming in Python, 
* ...are comfortable with basic calculus, probability, and linear algebra, 
* ...mastered Machine Learning 101, 
* ...have some familiarity with [pytorch](https://pytorch.org/), 
* ...are acquainted with Deep Learning 101. 

If you completed CS 5353/6353 (Deep Learning) or CS 5340/6340 (Natural Language Processing) or CS 5350/6350 (Machine Learning), I expect you will be able to keep up. 

We will spend the first two weeks going over background info and have a graded programming assigment relating to this in the first two weeks. You can give the course a try and if you struggle with the background concepts and the first homework, you can withdraw---students may drop a course within the first two weeks of a given semester without any penalties. 

If you'd like to revist and/or polish your knowledge, you can prepare by:

1. There are a ton of Python resources for people with some programming experience. Check them out [here](https://wiki.python.org/moin/BeginnersGuide/Programmers). [This](https://www.learnpython.org/) is a good one.

2. Math and machine learning basics are nicely covered in the first part of the [Deep Learning book](https://www.deeplearningbook.org/). Obviously, you can use the same book to familiarize yourself with deep learning, especially with the contents of Chapter 6 and Chapter 8 that are a must for this course. 

3. [Deep Learning with PyTorch: A 60 Minute Blitz](https://pytorch.org/tutorials/beginner/deep_learning_60min_blitz.html) (highly recommended)

4. [Practical Deep Learning for Coders by Fast.ai](https://course.fast.ai/) (3: Neural net foundations; 5: From-scratch model, 13: Backpropagation & MLP, 14: Backpropagation)


**Learning outcomes.** 



## Calendar

The calendar and readings are **tentative** and **subject to change**.

<table>
  <thead>
  <tr>
    <th>Date</th>
    <th>Theme</th>
    <th>Topic</th>
    <th>Lecture Materials</th>
    <th>Readings</th>
    <th>Work due</th>
  </tr>
  </thead>
  <tbody>
  {% for week in site.data.calendar %}
    {% for day in week.days %}
      <tr>
        <td>{{day.date}}</td>
        <td class="cal-content">{{day.theme}}</td>
        <td class="cal-content">{{day.topics}}</td>
        <td class="cal-content">
          {% if day.recording %}
            <a href="{{day.recording}}" class="cal-content-link">[recording]</a>
          {% endif %}
          {% if day.slides %}
            <a href="{{day.slides}}" class="cal-content-link">[slides]</a>
          {% endif %}
          {% if day.notes %}
            <a href="{{day.notes}}" class="cal-content-link">[notes]</a>
          {% endif %}
        </td>
        <td class="cal-content">{{day.readings}}</td>
        <td class="cal-content">{{day.due}}</td>
      </tr>
    {% endfor %}
  {% endfor %}
  </tbody>
</table>