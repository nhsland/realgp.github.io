---
permalink: "/shared-decision-options/"
layout: default
title:  "Shared Decision Options"
description: Shared Decision options
---

<section id="action" class="responsive">
        <div class="vertical-center">
             <div class="container">
                <div class="row">
                    <div class="action take-tour">
                            <center><h1 class="title">{{ page.title }}</h1>
                            <p>{{ page.description }}</p></center>
                    </div>
                </div>
            </div>
        </div>
   </section>

<section id="clinician">
      <div class="container">
        <div class="row">
          <div class="col-lg-12">
<br>
<br>

  	<div style="overflow-x:auto;">	
         <table id="project" class="table table-striped table-bordered display responsive no-wrap" style="width:100%">
        <thead>
            <tr>
                <th>Category</th>
                <th>Title</th>
                <th>Description</th>
                <th>Link</th>
                <th>Key Words</th>
            </tr>
        </thead>
        <tbody>
        {% for patients in site.patients %}
            <tr>
                <td style="text-align:center; vertical-align:middle">
                <a href="#" data-toggle="tooltip" title="{{ patients.category-desc }}">{{ patients.category }}</a>
                </td>
                <td><p>{{ patients.title }}</p></td>
                <td><p>{{ patients.description }}</p></td>
                <td style="text-align:center; vertical-align:middle">
                {% if patients.audio == null %}
                {% else %}
                <a href="{{ patients.audio }}" target="_blank"><img src="/img/itunes.png" width="80%"></a>
                {% endif %}
                {% if patients.article == null %}
                {% else %}
                <a href="{{ patients.article }}" target="_blank"><img src="/img/note.png" width="80%"></a>
                {% endif %}
                {% if patients.www == null %}
                {% else %}
                <a href="{{ patients.www }}" target="_blank"><img src="/img/globe.png" width="80%"></a>
                {% endif %} 
                {% if patients.youtube ==null %}
                {% else %}
                <a href="{{ patients.youtube }}" target="_blank"><img src="/img/video.png" width="80%"></a>
                {% endif %}
                </td>
                <td>{{ patients.keywords }}</td>
            </tr>
        {% endfor %}
    </tbody>
</table>
</div>

        
      </div>
	  </div>
	  </div>
    </section>
