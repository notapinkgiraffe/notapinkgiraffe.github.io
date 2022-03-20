---
title: Projects
layout: collection
<!-- layout: projects -->
permalink: /projects/
<!-- collection: staff_members -->
limit: 10
projects_layout: grid

show_excerpts: false
<!-- title: Recipes -->
<!-- layout: collection -->
<!-- permalink: /recipes/ -->
collection: projects
entries_layout: grid
---

I also compile projects [on a database](https://airtable.com/tblK4d66Lz55tKSD9/viw5YjxRKNJ7NKubn) if you're into that.

## Active/Ongoing

<!-- Enable when done with the rest of the page lol
<iframe class="airtable-embed" src="https://airtable.com/embed/shreTIW6QYdmraoJL?backgroundColor=transparent&viewControls=on" frameborder="0" onmousewheel="" width="100%" height="533" style="background: transparent; border: 1px solid #ccc;"></iframe>
-->

## Retired

<!-- Enable when done with the rest of the page lol
<iframe class="airtable-embed" src="https://airtable.com/embed/shrZLo5GTpOMaap9T?backgroundColor=transparent&viewControls=on" frameborder="0" onmousewheel="" width="100%" height="533" style="background: transparent; border: 1px solid #ccc;"></iframe>
-->

## All Projects

 {% for project in site.projects %}
  <h2>{{ project.title }}</h2>
  <p>{{ project.excerpt | markdownify }}</p>
 {% endfor %}

---

Sample document listing for the collection `_recipes`.

{% for staff_member in site.staff_members %}
  <h2>{{ staff_member.name }} - {{ staff_member.position }}</h2>
  <p>{{ staff_member.content | markdownify }}</p>
{% endfor %}
