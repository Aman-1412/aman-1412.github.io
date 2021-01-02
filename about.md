---
title: About
layout: page
---

# Aman Goyal

![Profile Image]({% if site.external-image %}{{ site.picture }}{% else %}{{ site.url }}/{{ site.picture }}{% endif %})

<p>Data-driven programmer having 2+ years of experience in Big Data and Data Science with a key focus on deliveries. Delivered valuable insights for the FX clients at HSBC. Advanced knowledge in Machine Learning, Python and InfoSec.</p>


<p>My abilities as a Data Scientist are rooted in a sturdy education during my university days. I did my bachelor's degree at the prestigious L D College of Engineering under Gujarat Technological University where I studied Information Technology. My university provided me ample opportunities to showcase my skills in Data Science - in terms of state-level exhibitions and competitions, and university level project showcases. With that practical experience and my internship in the early days, I found myself maturing in this field quite earlier.</p>

<h2>Skills</h2>

<ul class="skill-list">
	<li>Python</li>
	<li>GCP</li>
	<li>AWS</li>
	<li>Flask</li>
	<li>FastAPI</li>
	<li>PostgreSQL</li>
	<li>MongoDB</li>
	<li>Scrum and Kanban</li>
	<li>TDD</li>
	<li>Git</li>
</ul>

<h2>Data Science</h2>

<ul class="skill-list">
	<li>Machine Learning</li>
	<li>Deep Learning</li>
	<li>Tensorflow</li>
	<li>Pytorch</li>
	<li>NLP</li>
	<li>Computer Vision</li>
</ul>

<h2>Projects</h2>

<section class="list">
    {% for post in site.posts %}
        {% if post.projects %}
            <div class="item">
                <a class="url" href="{% if post.externalLink %}{{ post.externalLink }}{% else %}{{ site.url }}{{ post.url }}{% endif %}">
                    <h3 class="title">{{ post.title }}</h3>
                </a>
            </div>
        {% endif %}
    {% endfor %}
</section>