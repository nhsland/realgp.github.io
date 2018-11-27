---
permalink: "/clinical-skills/"
layout: page
title:  "Clinical Skills"
description: Real role play scenarios for your clinical skills assessment study group.
---

<!--<section class="bg-primary text-white" id="about">
      <div class="container text-center">
        <h2 class="mb-4">{{ page.title }}</h2>
        <h3 class="mb-4">{{ page.description }}</h3>
        <p align="left"></p>
		<center><a class="btn btn-light btn-xl" href="mailto:info@code4health.org?Subject=%5BSuggest%20New%20Topic%5D&Body=%5BName%5D%0A%5BRole%20%26%20Topic%5D%0A%5BDetails%20%5D%0A">Suggest a Topic</a></center>
</div>
</section>-->

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
                <th>Curriculum Area</th>
                <th>Title</th>
                <th>Description</th>
                <th>Audio/Video</th>
                <th>Patient Script</th>
                <th>Doctor's Notes</th>
                <th>Examination Findings</th>
                <th>LEJOG map</th>
                <th>Mapping the doctors words</th>
                <th>Transcription</th>
                <th>Key Words</th>
            </tr>
        </thead>
        <tbody>
        {% for clinician in site.clinicians %}
        {% if clinician.area contains page.title %}
            <tr>
                <!--category-->
                <td style="text-align:left; vertical-align:middle">
                <a href="#" data-toggle="tooltip" title="{{ clinician.category-desc }}">{{ clinician.category }}</a>
                </td>
                <!--title-->
                <td><p>{{ clinician.title }}</p></td>
                <!--description-->
                <td><p>{{ clinician.description }}</p></td>
                <!--audio and video-->
                <td style="text-align:center; vertical-align:middle">
                {% if clinician.audio == null %}
                {% else %}
                <a href="{{ clinician.audio }}" target="_blank"><img src="/img/itunes.png" width="23px"></a>
                {% endif %}
                {% if clinician.youtube ==null %}
                {% else %}
                <a href="{{ clinician.youtube }}" target="_blank"><img src="/img/video.png" width="23px"></a>
                {% endif %}
                </td>
                <!--Patient Script-->
                <td style="text-align:center; vertical-align:middle">
                {% if clinician.patient-script == null %}
                {% else %}
                <a href="{{ clinician.patient-script }}" target="_blank"><img src="/img/people.png" width="23px"></a>
                {% endif %}
                </td>
                <!--Doctors Note-->
                <td style="text-align:center; vertical-align:middle">
                {% if clinician.doctors-note == null %}
                {% else %}
                <a href="{{ clinician.doctors-note }}" target="_blank"><img src="/img/clinician.png" width="23px"></a>
                {% endif %}
                </td>
                <!--Examination Findings-->
                 <td style="text-align:center; vertical-align:middle">
                {% if clinician.findings == null %}
                {% else %}
                <a href="{{ clinician.findings }}" target="_blank"><img src="/img/note.png" width="23px"></a>
                {% endif %}
                </td>
                <!--LEJOG map-->
                 <td style="text-align:center; vertical-align:middle">
                {% if clinician.lejog == null %}
                {% else %}
                <a href="{{ clinician.lejog }}" target="_blank"><img src="/img/note.png" width="23px"></a>
                {% endif %}
                </td>
                <!--Mapping the doctors word-->
                 <td style="text-align:center; vertical-align:middle">
                {% if clinician.doctors-word == null %}
                {% else %}
                <a href="{{ clinician.doctors-word }}" target="_blank"><img src="/img/note.png" width="23px"></a>
                {% endif %}
                </td>
                <!--Transcription-->
                 <td style="text-align:center; vertical-align:middle">
                {% if clinician.transcription == null %}
                {% else %}
                <a href="{{ clinician.transcription }}" target="_blank"><img src="/img/note.png" width="23px"></a>
                {% endif %}
                </td>
                <!--Keywords-->
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
