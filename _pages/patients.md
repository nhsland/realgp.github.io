---
permalink: "/patients/"
layout: page
title:  "Patients"
---

<section class="bg-primary text-white" id="about">
      <div class="container text-center">
        <h2 class="mb-4">Patient Resources</h2>
        <p align="left">How often have you left the doctor's surgery thinking that you haven't</p>
		
		<p align="left">Add sub text if required</p><br>
		<center><a class="btn btn-light btn-xl" href="mailto:info@code4health.org?Subject=%5BSuggest%20New%20Community%5D&Body=%5BName%5D%0A%5BRole%20%26%20Organisation%5D%0A%5BDetails%20of%20the%20community%20and%20its%20aims%5D%0A%5BRelevant%20social%20media%20feeds%5D%0A%5BAny%20relevant%20partners/community%20members%5D%0A%5BLinks%20to%20any%20code%20repositories%20%28if%20applicable%29%5D%0A">Suggest a Topic</a></center>
</div>
</section>

<section id="patients">
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
        {% for patients in site.patients %}
            <tr>
                <td style="text-align:center; vertical-align:middle">{{ patients.category }}</td>
                <td><p>{{ patients.description }}</p></td>
                <td style="text-align:center; vertical-align:middle">
                <a href="{{ patients.audio1 }}">{{patients.audio1-desc }}</a><br>
                <a href="{{ patients.audio2 }}">{{patients.audio2-desc }}</a><br>
                <a href="{{ patients.audio3 }}">{{patients.audio3-desc }}</a><br>
                </td>  
                <td style="text-align:center; vertical-align:middle">
                <a href="{{ patients.decision-aid1 }}">{{ patients.decision-aid1-desc }}</a><br>
                <a href="{{ patients.decision-aid2 }}">{{ patients.decision-aid2-desc }}</a><br>
                <a href="{{ patients.decision-aid3 }}">{{ patients.decision-aid3-desc }}</a><br>
                </td>    
                <td style="text-align:center; vertical-align:middle">
                <a href="{{ patients.www1 }}">{{ patients.www1-desc }}</a><br>
                <a href="{{ patients.www2 }}">{{ patients.www2-desc }}</a><br>
                <a href="{{ patients.www3 }}">{{ patients.www3-desc }}</a><br>
                </td>
                <td style="text-align:center; vertical-align:middle">
                {% if patients.forum == null %}
                {% else %}
                <a href="{{ patients.forum }}" target="_blank"><i class="fas fa-comments fa-2x"></i></a>
                {% endif %}
                {% if patients.email == null %}
                {% else %}
                <a href="mailto:{{ patients.email }}"><i class="fas fa-envelope fa-2x"></i></a>
                {% endif %}
                {% if patients.twitter == null %}
                {% else %}
                <a href="http://twitter.com/{{ patients.twitter }}" target="_blank"><i class="fab fa-twitter fa-2x"></i></a>
                {% endif %}
                {% if patients.facebook == null %}
                {% else %}
                <a href="{{ patients.facebook }}" target="_blank"><i class="fab fa-facebook fa-2x"></i></a>
                {% endif %}
                {% if patients.youtube ==null %}
                {% else %}
                <a href="{{ patients.youtube }}" target="_blank"><i class="fab fa-youtube fa-2x"></i></a>
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
