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

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}

Through **<span style="color: black;">this website</span>** we will share only the schedule and materials. Everything else---syllabus, announcements, discussion, turning in assignments/project components, communicating grades, policies---will be done through **<span style="color: black;">Canvas</span>**.

Please use the Canvas discussion forum as the preferred medium for interacting with the instructor and the teaching assistants rather than emailing/messaging directly. Take advantage of the instructor hours. We will work hard to be accessible to students. Don't be shy if you don’t understand something: come to office hours, post in the forum, or speak up in class!

## Description

Data mining is the study of efficiently finding structures and patterns in large data sets. We will focus on several aspects of this: (1) converting from a messy and noisy raw data set to a structured and abstract one, (2) applying scalable and probabilistic algorithms to these well-structured abstract data sets, and (3) formally modeling and understanding the error and other consequences of parts (1) and (2), including choice of data representation and trade-offs between accuracy and scalability. These steps are essential for training as a data scientist.

Algorithms, programming, probability, and linear algebra are required tools for understanding these approaches.

Topics will include: similarity search, clustering, regression/dimensionality reduction, graph analysis, PageRank, and small space summaries. We will also cover several recent developments, and the application of these topics to modern applications, often relating to large internet-based companies.

Upon completion, students should be able to read, understand, and implement ideas from many data mining research papers.


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