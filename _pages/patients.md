---
permalink: "/patients/"
layout: page
title:  "Patients"
---

<section class="bg-primary text-white" id="about">
      <div class="container text-center">
        <h2 class="mb-4">Patient Resources</h2>
        <p align="left">How often have you left the doctor’s surgery thinking that you haven’t had enough time to fully explore what is the best option to manage your problem? We are all individuals. We all make different decisions about what we are happy to do to keep healthy. </p>
        <p align="left">We still depend on doctors to help us to figure out what our illnesses are. And when we figure out what our illness is, we all need help to negotiate what types of treatment suit us best. What works best to help us to feel better or live longer? What are we prepared to do? Figuring all of this out takes time. Your 10 minute GP appointment rarely suffices. Let your doctor help you to decide what your problem is. Then, join me in bringing your choices to life.</p>
        <p align="left">I’ve had conversations with some of my patients about their choices, based on what I have discovered about their circumstances, values, fears and wishes. I present viable options to them based on the things that matter to them. Together, the patient and I can tailor potential treatment options to their condition or problem. I present extra evidence to help you, the listening audience, to make decisions that might suit you too.</p>
        <p align="left">Most GPs will ask you to read more about your problem before deciding what to do, to make you feel better. My experience is that many patients struggle to bring their choices to life from written words. When I share these audio recordings with my patients, they quickly make their own choices, and usually they contact me by phone to take the next steps.</p>
        <p align="left">There is no single “best” option that suits every patient. Just like some children prefer swings, some children prefer roundabouts. I have recorded these extended conversations with real patients to illustrate the broad range of options available to patients who have a similar diagnosis or problem.</p>
        <p align="left">These audios are part of our Real General Practice project. Real General Practice aims to help GPs in training, and GPs, to improve their communication skills and their knowledge of how to to their job in the consulting room. Perhaps you could make a recommendation to your friends on social media to ensure that more patients get to access our shared decision making tools </p>
		<center><a class="btn btn-light btn-xl" href="mailto:info@code4health.org?Subject=%5BSuggest%20New%20Topic%5D&Body=%5BName%5D%0A%5BRole%20%26%20Topic%5D%0A%5BDetails%20%5D%0A">Suggest a Topic</a></center>
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
                <th>Link</th>
                <th>Key Words</th>
            </tr>
        </thead>
        <tbody>
        {% for patients in site.patients %}
            <tr>
                <td style="text-align:center; vertical-align:middle"><a href="{{ patients.page }}">{{ patients.category }}</a></td>
                <td><p>{{ patients.description }}</p></td>
                <td style="text-align:center; vertical-align:middle">
                {% if patients.audio == null %}
                {% else %}
                <a href="{{ patients.audio }}" target="_blank"><i class="fas fa-headphones fa-2x"></i></a>
                {% endif %}
                {% if patients.article == null %}
                {% else %}
                <a href="{{ patients.article }}" target="_blank"><i class="fas fa-file-alt fa-2x"></i></a>
                {% endif %}
                {% if patients.www == null %}
                {% else %}
                <a href="{{ patients.www }}" target="_blank"><i class="fas fa-globe fa-2x"></i></a>
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
