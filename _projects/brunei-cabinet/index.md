---
title: "Brunei Cabinet Database"
layout: project
permalink: /brunei-cabinet/
thumb: /projects/images/bruneicabinet_db_201802.png
thumb-150: /projects/images/bruneicabinet_db_150x150.png
thumb-300: /projects/images/bruneicabinet_db_300x200.png
categories:
  - Projects
tags:
  - government
  - tools - Airtable
last_modified_at: 2022-02-20T00:05:00+08:00
proj_status: Ongoing
proj_years: 2015 - Present
proj_tools: Airtable, Google Sheets
proj_featured: true
proj_url: http://bit.ly/brucabinet_base
text_excerpt: "Database of current, as well as previous, Brunei Cabinet members (Ministers, Deputy Ministers, and positions with Ministerial Ranks).
Also includes Permanent Secretaries and Deputy Permanent Secretaries."
share: true
lightbox: true
---

Database of current, as well as previous, Brunei Cabinet members (Ministers, Deputy Ministers, and positions with Ministerial Ranks). 
Also includes Permanent Secretaries and Deputy Permanent Secretaries.

[Visit database](#link){: .btn .btn--primary .btn--small}
[About this project](projects/brunei_cabinet){: .btn .btn--accent .btn--small}

Shortcuts:  
[List](#link){: .btn .btn--inverse .btn--small} Council of Cabinet Ministers only  
[List](#link){: .btn .btn--inverse .btn--small} Women Senior Government Officials

{% include toc %}

## What Brunei Cabinet info are you looking for?

{% if site.data.proj-sublinks %}
{% assign main_id = 'brucabinetdbSublinks' %}
<div class="accordion" id="{{ main_id }}" style="width:90%; margin-left: auto; margin-right: auto">

  {%- for link in site.data.proj-sublinks -%}
  {%- if link.project == 'brucabinetdb' -%}
    {%- assign id = link.project | append: link.id -%}
    
  <div class="accordion-item">
    <h2 class="accordion-header" id="{{ link.project }}{{ link.id }}">
      <button class="accordion-button{% unless link.id == 1 %} collapsed{% endunless %}" type="button" data-bs-toggle="collapse" data-bs-target="#collapse{{ id }}" aria-expanded="true" aria-controls="collapseOne">
        {{ link.title }}
      </button>
    </h2>
    <div id="collapse{{ id }}" class="accordion-collapse collapse{% if link.id == 1 %} show{% endif %}"
    aria-labelledby="{{ id }}" data-bs-parent="#brucabinetdbSublinks">
      <div class="accordion-body">
      
      {%- if link.url contains '://' -%}
        {%- assign url = link.url -%}
      {%- else -%}
        {%- assign url = link.url | relative_url -%}
      {%- endif -%}
      
      <figure style="width: 450px" class="align-left">
        <a href="{{ link.image | absolute_url }}">
        <img src="{{ link.image | absolute_url }}" alt="{{ link.image_alt }}">
        </a>
        <figcaption>{{ link.caption }}</figcaption>
      </figure> 
      
      <p><a href="{{ url | absolute_url }}" class="btn btn--primary btn--small">{{ link.button_title }}</a></p>
      
      <p>{{ link.description }}</p>
      
      {% if link.notice %}
      [card]{{ link.notice }}
      {% endif %}
      
      </div>
    </div>
  </div>
  {%- endif -%}
  {%- endfor -%}
</div>
{% endif %}

---

## About

### Overview

Database of current, as well as previous, Brunei Cabinet members (Ministers, Deputy Ministers, and positions with Ministerial Ranks). 
Also includes Permanent Secretaries and Deputy Permanent Secretaries.

Info that's recorded in the database:

* Appointment details (Date started, date ended, references)
* Person details (Name, age, background, photo) - _Publicly available information only_

### Not a Feature: <u>Titles & Hierarchies</u>

Apologies that the titles of individuals ~~and the appropriate ~~hierarchies of Ministries~~ \* may not be 
shown correctly. This is not meant to offend, it's to make the database simpler to manage.

\* - _As of Jan 2018, Ministry hierarchy has been added (and is hopefully working)_

### Features: <u>Database Views</u>

You can view the **Current Cabinet**:

<a class="button btn80px" href="https://airtable.com/shrmqBAoPH5rhwWBj/tblR9UtkFralfbHvy">View Gallery</a> Cabinet Ministers only  
<a class="button btn80px" href="https://airtable.com/shro4B3NhGBfkwKOG">View List</a> All including PermSecs

The database is meant to be a reference to current and past appointments. Other than that, I also thought it would be useful to have 
certain kinds of information (i.e. database views/queries) about Brunei senior government appointments, such as...

* [Gallery of women appointed (Current)](https://airtable.com/shrwrDNEJ8Zb11z8c)  
* [List of women appointed (Current & Past)](https://airtable.com/shrOGuC4eU2pU9f38)  
* [Age at appointment](https://airtable.com/shrICwXbjtpjZww8h)
* [Length of current appointments](https://airtable.com/shrB1Msu7dw2nMb0z)
* History of appointments in a Ministry (e.g. PMO)  
* History of appointments for a person

<div class="list-group">
  <a href="#" class="list-group-item list-group-item-action d-flex gap-3 py-3" aria-current="true">
    <img src="https://github.com/twbs.png" alt="twbs" width="32" height="32" class="rounded-circle flex-shrink-0">
    <div class="d-flex gap-2 w-100 justify-content-between">
      <div>
        <h6 class="mb-0">List group item heading</h6>
        <p class="mb-0 opacity-75">Some placeholder content in a paragraph.</p>
      </div>
      <small class="opacity-50 text-nowrap">now</small>
    </div>
  </a>
  <a href="#" class="list-group-item list-group-item-action d-flex gap-3 py-3" aria-current="true">
    <img src="https://github.com/twbs.png" alt="twbs" width="32" height="32" class="rounded-circle flex-shrink-0">
    <div class="d-flex gap-2 w-100 justify-content-between">
      <div>
        <h6 class="mb-0">Another title here</h6>
        <p class="mb-0 opacity-75">Some placeholder content in a paragraph that goes a little longer so it wraps to a new line.</p>
      </div>
      <small class="opacity-50 text-nowrap">3d</small>
    </div>
  </a>
  <a href="#" class="list-group-item list-group-item-action d-flex gap-3 py-3" aria-current="true">
    <img src="https://github.com/twbs.png" alt="twbs" width="32" height="32" class="rounded-circle flex-shrink-0">
    <div class="d-flex gap-2 w-100 justify-content-between">
      <div>
        <h6 class="mb-0">Third heading</h6>
        <p class="mb-0 opacity-75">Some placeholder content in a paragraph.</p>
      </div>
      <small class="opacity-50 text-nowrap">1w</small>
    </div>
  </a>
</div>

### Contribute!

Currently, I've collected appointments during the 2010-2015 and 2015-2010 periods. There are still many gaps that 
I try to update in my spare time.

If you'd like to help contribute, I'd greatly appreciate it! (Crowdsourcing is A++, guys)

* [Submit Appointment](http://bit.ly/brucabinet_submitinfo)
* [Submit Photo or Biography](http://bit.ly/brucabinet_submitbio)



## Background

### Iterations

#### Part 1: Spreadsheet

To keep track of 'who replaced who' in the 2015 Brunei Cabinet reshuffle, I started a **spreadsheet** on Google Sheets.
I ended up also tracking appointments of Permanent Secretaries and their Deputies. The further back 
I dug, the larger the spreadsheet became.

* Status: **Retired**. Spreadsheet remains online but will not be updated.  
* Visit Spreadsheet: http://goo.gl/upuDCH

#### Part 2: Database

The spreadsheet got unwieldy, so when I discovered Airtable, I experimented with the data in a database format. 
I liked it so much that I ended up transferring it over from the spreadsheet to the database. 
(Databases are a lot of fun.)

* Status: **Current**  
* Visit Database: http://bit.ly/brucabinet_base

### Inspirations

It's worth mentioning that although [SiapaKedia](http://siapakedia.com.bn/) by BAG Networks was not a direct inspiration for this project, I had used it occasionally as a resource for checking appointments and "who's who" of senior government officials. It was pretty thorough!

When I created my spreadsheet, SiapaKedia had already started to be inactive. I decided to make my spreadsheet that would fit my specific interest, i.e. a resource that would show me who had been transferred, promoted, and so on.

&nbsp;

----

### Meta

Updates to the database are now posted [here on my project status database](https://airtable.com/shrXOQm7uSgp469Aa).

Previous updates and posts on my Tumblr:

* [General project announcements](http://rolluptheclouds.tumblr.com/tagged/brunei-cabinet)
* [Meta posts](http://rolluptheclouds.tumblr.com/tagged/brunei-cabinet-meta), i.e. the smaller updates
* [Posts specific to Database](http://rolluptheclouds.tumblr.com/tagged/brunei-cabinet-database) (Part 2 - current)
* [Posts specific to Spreadsheet](http://rolluptheclouds.tumblr.com/tagged/brunei-cabinet-spreadsheet) (Part 1)
