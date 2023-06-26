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
MoWe / 4:35-5:55 PM	, [WEB 1230](https://map.utah.edu/index.html?code=WEB) 
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

---

Through this website we will share:
* [Schedule](https://utah-explainability.github.io/#calendar) & lecture materials (slides, recordings)
* Info about [paper discussions]() and [projects]()
* [Info that might be useful before enrolling](https://utah-explainability.github.io/#faq-before-enrolling)

Syllabus, announcements, communicating grades, policies is shared on **<span style="color: black;">Canvas</span>**. Communication will be done through **<span style="color: black;">Piazza</span>**. You will turn in your assignments to **<span style="color: black;">Gradescope</span>**.

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

## FAQ Before Enrolling

### What will you learn in this course? 

### Which modalities does this course cover?
We will almost exclusively talk about **applications in NLP (so text)** and in computer vision with **static images**. Inputs in these domains are represented with [embeddings](https://course18.fast.ai/lessonsml1/lesson11.html)---high-dimensional vectors of floating point numbers whose individual dimensions are not interpretable. If you are interested in applications that fall under data science, you will instead likely work with "meaningful" features such as income of a person or zip code of a certain location. This course is not about such applications. We hope you find the course useful even if the data you work with is handled differently from text or images. We believe it can be inspiring to think whether these methods can be applied to a different domain, and realizing that they cannot, can be useful.


### Which machine learning models does this course cover?
We focus on deep learning models (deep neural networks) and we will almost solely talk about [transformer](http://jalammar.github.io/illustrated-transformer/)-based models. 

### Local vs. global explanations?
This course will **not** focus on [global methods](https://christophm.github.io/interpretable-ml-book/scope-of-interpretability.html) that analyze models'  behavior and internals such as [probing](https://nlp.stanford.edu/~johnhew/interpreting-probes.html). We focus on methods that answer questions such as: 

* Which part of the input led to assigning this label?             
* How to edit the input to change the model's answer to something else?                           
* In plain English, why is this input assigned this label?                   
* Which training examples caused the prediction?   

### Formal pre-requisites?
This course doesn't have formal pre-requisites because these days one can learn about machine learning and adjacent topics in many different ways, but we expected that you...

* ...are experienced with programming in Python, 
* ...are comfortable with basic calculus, probability, and linear algebra, 
* ...have solid machine learning foundations, 
* ...have some familiarity with [pytorch](https://pytorch.org/), 
* ...are acquainted with Deep Learning 101. 

If you completed CS 5353/6353 (Deep Learning) or CS 5340/6340 (Natural Language Processing) or CS 5350/6350 (Machine Learning), we expect you will be able to keep up. 

**<span style="color: black;">My advice:</span>** If you are interested in the course, **give it a  try**. We will spend the first two weeks going over the background and have a graded programming assignment about it. If you struggle with the background concepts and the first homework, you can withdraw---students may drop a course within the first two weeks of a given semester without any penalties. 


**<span style="color: black;">Revisiting/polishing your knowledge.</span>** You can prepare by:

1. There are a ton of Python resources for people with some programming experience. Check them out [here](https://wiki.python.org/moin/BeginnersGuide/Programmers). My colleagues suggest these: [1](https://www.learnpython.org/), [2](https://diveintopython3.net/), [3](https://snakify.org/en/), and [4](https://runestone.academy/ns/books/published/thinkcspy/index.html?mode=browsing).

2. Math and machine learning basics are nicely covered in the first part of the [Deep Learning book](https://www.deeplearningbook.org/). Obviously, you can use the same book to familiarize yourself with deep learning, especially with the contents of Chapter 6 and Chapter 8 that are a must for this course. 

3. [Deep Learning with PyTorch: A 60 Minute Blitz](https://pytorch.org/tutorials/beginner/deep_learning_60min_blitz.html) (highly recommended)

4. [Practical Deep Learning for Coders by Fast.ai](https://course.fast.ai/) (3: Neural net foundations; 5: From-scratch model, 13: Backpropagation & MLP, 14: Backpropagation)


