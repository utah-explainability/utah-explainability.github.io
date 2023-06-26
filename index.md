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

Syllabus, announcements, communicating grades, policies, etc. are shared on **<span style="color: black;">Canvas</span>**. Communication will be done through **<span style="color: black;">Piazza</span>**. You will turn in your assignments to **<span style="color: black;">Gradescope</span>**.

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

* **Train a transformer-based model** for an NLP or computer vision application, **obtain its predictions**, and apply common explainability methods (covered in lectures) to **explain the predictions**. Four <u>homework assignments</u> are designed to work on this. 

* **Define utility/function of an explanation for a given application.** This course should teach you to ask: “What will best accomplish the explanatory functions [I hope to achieve in this case]?” (specific; application-based) instead of “Is this an appropriate explanation [in this case]?” (generic; very common in current ML research). A successful <u>project proposal</u>  (a component of the grade) has to define an appropriate function.

* **Identify and apply a method that creates appropriate explanations for a desired utility/function.** A successful <u>intermediate project status</u> report should identify such a method.

* Conduct a **user study** to evaluate produced explanations based on their utility. The course has a <u>dedicated session</u> for preparing an interface for a user study and <u>another session</u> for conducting it with class peers. Having a user study ready ready for the class is a component of the project grade as well as a successful <u>final project presentation</u> that shows how well explanations accomplish the explanatory function according to the study.

* **Read cutting-edge research publications** requiring being acquainted with the principles and concepts of explainable ML. There will be <u>six class sessions devoted to paper discussions</u>. This part of the course will be organized as a role-playing paper reading seminar with 5 regular roles: original author, scientific peer reviewer, archaeologist, imaginative researcher, and original author of a related paper. Those who are not assigned to be the official presenters will either play a wild card role (any role they’d like to be, such as an industry practitioner, a cranky researcher, etc.) or complete a written artifact (a study notes, a blog post, an opinion piece, a scribe of the class discussion). This format requires everyone to actually read the papers and engage in the discussion about them. The paper discussion is one of the main components of the grade. 

* Follow an *ACL/EMNLP (leading NLP conferences) review style to properly **review a research paper** on explainable ML. One of the roles in the role-playing paper discussion is “scientific peer reviewer”. You will <u>take that role once</u> and your review will contribute to your paper discussion grade. 


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


