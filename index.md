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

**What modalities does this course cover?** We will almost exclusively talk about **applications in NLP** and computer vision for **static images**. Inputs in these domains are represented with [embeddings](https://course18.fast.ai/lessonsml1/lesson11.html)--high-dimentsional vectors of floating point numbers whose individual dimensions are not interpretable. In other domains, typically in applications that fall under data science, you might work with "meaningful" features such as income or zip code. This course is not about such applications. 

**What machine learning models this course covers?** We focus on deep learning models (deep neural networks) and we will almost solely focus on the [transformer](http://jalammar.github.io/illustrated-transformer/)-based models.  

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