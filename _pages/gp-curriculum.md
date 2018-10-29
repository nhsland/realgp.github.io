---
permalink: "/GP-curriculum/"
layout: page
title:  "GP Curriculum"
description: Share our Consultations from across the GP curriculum 
---

<section class="bg-primary text-white" id="about">
      <div class="container text-center">
        <h2 class="mb-4">{{ title }}</h2>
        <h3 class="mb-4">{{ description }}</h3>
        <p align="left"></p>
		<center><a class="btn btn-light btn-xl" href="mailto:info@code4health.org?Subject=%5BSuggest%20New%20Topic%5D&Body=%5BName%5D%0A%5BRole%20%26%20Topic%5D%0A%5BDetails%20%5D%0A">Suggest a Topic</a></center>
</div>
</section>

<section id="clinician">
      <div class="container">
        <div class="row">
          <div class="col-lg-12">
            <center><h2 class="section-heading">Patient Resources</h2>
            <hr class="my-4"></center>

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
        {% for clinician in site.clinician %}
        {% if clinician.category == page.title %}
            <tr>
                <td style="text-align:center; vertical-align:middle">
                <a href="#" data-toggle="tooltip" title="{{ clinician.category-desc }}">{{ clinician.category }}</a>
                </td>
                <td><p>{{ clinician.title }}</p></td>
                <td><p>{{ clinician.description }}</p></td>
                <td style="text-align:center; vertical-align:middle">
                {% if clinician.audio == null %}
                {% else %}
                <a href="{{ clinician.audio }}" target="_blank"><i class="fas fa-headphones fa-2x"></i></a>
                {% endif %}
                {% if clinician.article == null %}
                {% else %}
                <a href="{{ clinician.article }}" target="_blank"><i class="fas fa-file-alt fa-2x"></i></a>
                {% endif %}
                {% if clinician.www == null %}
                {% else %}
                <a href="{{ clinician.www }}" target="_blank"><i class="fas fa-globe fa-2x"></i></a>
                {% endif %} 
                {% if clinician.youtube ==null %}
                {% else %}
                <a href="{{ clinician.youtube }}" target="_blank"><i class="fab fa-youtube fa-2x"></i></a>
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
