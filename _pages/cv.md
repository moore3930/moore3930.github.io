---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* M.S. in EECS, Peking University, 2018
* B.S. in CS, Hefei University of Technology, 2015

Work experience
======
* *Spring 2020 - now: Senior Algorithm Engineer, DuerOS, Baidu, Beijing*
  * designed and built a fast non-autoregressive model for joint intent detection and slot filling, named 
  [*SlotRefine*](https://arxiv.org/pdf/2010.02693.pdf), which achieves better performance and efficiency for online
  [*DuerOS*](https://dueros.baidu.com/en/index.html) system.
  * Now, I focus on how to build a robust flat semantic pasring (e.g. Slot Filling) system to help DuerOS be 
  less disturbed by noise.

* *Summer 2018 - Fall 2019: Algorithm Engineer, Searching & Recommendation Group, Alibaba, Beijing*
  * Designed and built a distributed deep learning tool, named DeepI2I, to extract item embeddings for 
  [*Taobao*](https://www.taobao.com/)  which is the largest e-commerce platform in China and has more than 3 billions 
  various commodities. DeepI2I works great and helps with recommendation tasks in other subsidiaries of Alibaba.
  * Integrated GCN technology into a transformer architecture to improve ranking results of the recommendation system.
 
* *Summer 2017 - spring 2018: Intern, XiaoIce Team, Microsoft, Beijing*
  * Designed and built a model to give XiaoIce the ability to make diversity comments on sports news using
   a generation method.

Publications
======
  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
