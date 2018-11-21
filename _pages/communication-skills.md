---
permalink: "/communication-skills/"
layout: default
title:  "Communication Skills"
description: Communication skills learning
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
                <th>Associated Files</th>
                <th>Key Words</th>
            </tr>
        </thead>
        <tbody>
        {% for clinician in site.clinicians %}
        {% if clinician.area contains page.title %}
     <tr>
                <td style="text-align:left; vertical-align:middle">
                <a href="#" data-toggle="tooltip" title="{{ clinician.category-desc }}">{{ clinician.category }}</a>
                </td>
                <td><p>{{ clinician.title }}</p></td>
                <td><p>{{ clinician.description }}</p></td>
                <td style="text-align:center; vertical-align:middle">
                {% if clinician.audio == null %}
                {% else %}
                <a href="{{ clinician.audio }}" target="_blank"><img src="/img/itunes.png" width="23px"></a>
                {% endif %}
                {% if clinician.article == null %}
                {% else %}
                <a href="{{ clinician.article }}" target="_blank"><img src="/img/note.png" width="23px"></a>
                {% endif %}
                {% if clinician.map == null %}
                {% else %}
                <a href="{{ clinician.www }}" target="_blank"><img src="/img/map.png" width="23px"></a>
                {% endif %} 
                {% if clinician.ljog ==null %}
                {% else %}
                <a href="{{ clinician.ljog }}" target="_blank"><img src="/img/LJOG.png" width="23px"></a>
                {% endif %}
                 {% if clinician.youtube ==null %}
                {% else %}
                <a href="{{ clinician.youtube }}" target="_blank"><img src="/img/video.png" width="23px"></a>
                {% endif %}
                </td>
                <td>{{ clinician.keywords }}</td>
            </tr>
            {% endif %}
        {% endfor %}
    </tbody>
</table>
</div>

        
      </div>
	  </div>
	  </div>
    </section>
