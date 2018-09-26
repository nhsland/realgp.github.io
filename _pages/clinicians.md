---
permalink: "/clinicians/"
layout: page
title:  "Clinicians"
---

<section class="bg-primary text-white" id="about">
      <div class="container text-center">
        <h2 class="mb-4">Clinician Resources</h2>
        <p align="left">Insert page description</p>
		
		<p align="left">Add sub text if required</p><br>
		<center><a class="btn btn-light btn-xl" href="mailto:info@code4health.org?Subject=%5BSuggest%20New%20Community%5D&Body=%5BName%5D%0A%5BRole%20%26%20Organisation%5D%0A%5BDetails%20of%20the%20community%20and%20its%20aims%5D%0A%5BRelevant%20social%20media%20feeds%5D%0A%5BAny%20relevant%20partners/community%20members%5D%0A%5BLinks%20to%20any%20code%20repositories%20%28if%20applicable%29%5D%0A">Suggest a Topic</a></center>
</div>
</section>

<section id="Clinicians">
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
                <th>Description</th>
                <th>Audio</th>
				<th>Shared decision aids or articles</th>
                <th>Useful Links</th>
                <th>Social</th>
                <th>Key Words</th>
            </tr>
        </thead>
        <tbody>
        {% for Clinicians in site.Clinicians %}
            <tr>
                <td style="text-align:center; vertical-align:middle">{{ Clinicians.category }}</td>
                <td><p>{{ Clinicians.description }}</p></td>
                <td style="text-align:center; vertical-align:middle">{{ Clinicians.audio }}</td>  <td style="text-align:center; vertical-align:middle">
                <a href="{{ Clinicians.decision-aid1 }}">{{ Clinicians.decision-aid1 }}</a><br>
                <a href="{{ Clinicians.decision-aid2 }}">{{ Clinicians.decision-aid2 }}</a><br>
                <a href="{{ Clinicians.decision-aid3 }}">{{ Clinicians.decision-aid3 }}</a><br>
                </td>    
                <td style="text-align:center; vertical-align:middle">
                <a href="{{ Clinicians.www1 }}">{{ Clinicians.www1 }}</a><br>
                <a href="{{ Clinicians.www2 }}">{{ Clinicians.www2 }}</a><br>
                <a href="{{ Clinicians.www3 }}">{{ Clinicians.www3 }}</a><br>
                </td>
                <td style="text-align:center; vertical-align:middle">
                {% if Clinicians.forum == null %}
                {% else %}
                <a href="{{ Clinicians.forum }}" target="_blank"><i class="fas fa-comments fa-2x"></i></a>
                {% endif %}
                {% if Clinicians.email == null %}
                {% else %}
                <a href="mailto:{{ Clinicians.email }}"><i class="fas fa-envelope fa-2x"></i></a>
                {% endif %}
                {% if Clinicians.twitter == null %}
                {% else %}
                <a href="http://twitter.com/{{ Clinicians.twitter }}" target="_blank"><i class="fab fa-twitter fa-2x"></i></a>
                {% endif %}
                {% if Clinicians.facebook == null %}
                {% else %}
                <a href="{{ Clinicians.facebook }}" target="_blank"><i class="fab fa-facebook fa-2x"></i></a>
                {% endif %}
                {% if Clinicians.youtube ==null %}
                {% else %}
                <a href="{{ Clinicians.youtube }}" target="_blank"><i class="fab fa-youtube fa-2x"></i></a>
                {% endif %}
                </td>
                <td>{{ Clinicians.keywords }}</td>
            </tr>
        {% endfor %}
    </tbody>
</table>
</div>

        
      </div>
	  </div>
	  </div>
    </section>
