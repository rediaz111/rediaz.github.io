---
title: Roberto Efraín Díaz
layout: default
group: cv
---
<h4 class="page-header text-center"> A complete version of my CV can be found [here](/static/pdf/Diaz_CV_2022.pdf "Link to PDF of Roberto Efraín Díaz's CV"){:target="_blank"}</h4>

<h1>Education</h1>
<div class="row">
<hr>
PhD Candidate, Biochemistry and Molecular Biology<br>
University of California, San Francisco<br>
**Thesis**: Structural characterization of pH-sensitive residues in mammalian chitinases<br>
**Advisor**: Dr. [James S. Fraser](https://fraserlab.com "Fraser Lab (opens in new tab)"){:target="_blank"}

Bachelor of Science with Honors, Neuroscience<br>
University of Miami<br>
**Thesis**: Modifying transcription factor CREB with transactivation domains VP16 and VP64 to increase neurite outgrowth<br>
**Advisor**: Dr. [Vance Lemmon](https://www.lembixlab.net "LemBix Lab (opens in new tab)"){:target="_blank"}
<hr>
</div>

<br>

<h1>Honors and Awards</h1>
<div class="row">
{% for award in site.cv reversed | sort: "date" %}
<hr>
<h4>{{award.title | markdownify | remove: '<p>' | remove: '</p>'}}</h4>
{{award.organization | markdownify | remove: '<p>' | remove: '</p>'}}
{% if award.description %}
{{award.description | markdownify | remove: '<p>' | remove: '</p>'}} <br>
{% endif %}
{% endfor %}
