---
permalink: "/clinicians/"
layout: default
title:  "Clinicians"
---
<section id="action" class="responsive">
        <div class="vertical-center">
             <div class="container">
                <div class="row">
                    <div class="action take-tour">
                            <center><h1 class="title">Clinician Resources</h1>
                            <p>Choose the best option for YOU, with our help</p></center>
                    </div>
                </div>
            </div>
        </div>
   </section>

<section id="services">
        <div class="container">
            <div class="row">
<p align="left">Real general practice is designed to help you to acquire the skills and knowledge necessary for you to pass the clinical skills assessment exam. It will demonstrate to you: how busy GPs incorporate up-to-date knowledge and evidence based, patient-centred practice into their consultations. CSA candidates and medical students will often prefer to use our material in study groups, with or without the support of a trainer. Busy GPs can bring themselves up-to-date listening to audio material on their smart phones wherever and whenever they feel so inclined.</p>
        <p align="left">This course consists of 4 groups of educational material</p>
        <ul align="left">
            <li align="left"> 1. Role play scenarios for your CSA study group</li>
            <li align="left"> 2. Communication skills learning. These are teaching sessions recorded with our communication skills experts to improve your consultations</li>
            <li align="left"> 3. Shared decision options. These are extended option discussions with patients with specific conditions. These recordings are suitable for GPs and patients alike</li>
             <li align="left">4. Consultations with patients with problems from all of the GP curriculum areas. This allows you to be comprehensive in your learning. And to tick some boxes in your e-portfolio.</li>
          </ul>
          <br><br> 
        </div>
    </div>
</section>

<section id="services">
     <div class="container">
            <div class="row">
                <div class="col-sm-4 text-center padding wow fadeIn" data-wow-duration="1000ms" data-wow-delay="600ms">
                    <div class="single-service">
                        <div class="wow scaleIn" data-wow-duration="500ms" data-wow-delay="600ms">
                            <a href="{{ '/clinicians_how2' }}"><img src="/img/clinician1.png" alt="">
                        </div>
                        <h2>How to use our resources</h2>
                        <p>Access our guides to each role and area</p></a>
                    </div>
                </div>
            </div>
        </div>
</section>

<!--<section id="clinician">
      <div class="container">
            <div class="row">
                <center><h1>How to use our resources</h1>
                <p>Choose the role or roles that apply to you and read or listen to the information provided</p></center>
                <hr class="my-4">
                <div class="col-lg-12">
                <br>
                <br>
  	                <div style="overflow-x:auto;">	
                        <table id="project" class="table table-striped table-bordered display responsive no-wrap" style="width:100%">
                     <thead>
                        <tr>
                            <th>Role</th>
                            <th>Title</th>
                            <th>Description</th>
                            <th>Link</th>
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
                            <a href="{{ clinician.audio }}" target="_blank"><img src="/img/itunes.png" width="80%"></a>
                            {% endif %}
                            {% if clinician.article == null %}
                            {% else %}
                            <a href="{{ clinician.article }}" target="_blank"><img src="/img/note.png" width="80%"></a>
                            {% endif %}
                            {% if clinician.www == null %}
                            {% else %}
                            <a href="{{ clinician.www }}" target="_blank"><img src="/img/globe.png" width="80%"></a>
                            {% endif %} 
                            {% if clinician.youtube ==null %}
                            {% else %}
                            <a href="{{ clinician.youtube }}" target="_blank"><img src="/img/video.png" width="80%"></a>
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
</section> -->

<section id="services">
        <div class="container">
                <div class="row">
                <center><h1>Resources</h1></center>
                <hr class="my-4">
                <div class="col-xs-4 col-sm-offset-3 col-sm-6 col-md-offset-0 text-center padding wow fadeIn" data-wow-duration="1000ms" data-wow-delay="600ms">
                    <div class="single-service">
                        <div class="wow scaleIn" data-wow-duration="500ms" data-wow-delay="600ms" height="200px">
                          <a href="{{ '/clinical-skills' }}"><img src="/img/people.jpg" title="Real role play scenarios for your Clinical Skills Assessment study group" height="100%"></a>
                        </div>
                        <h2>Clinical Skills</h2>
                        <p>Real role play scenarios for your Clinical Skills Assessment study group.</p>
                    </div>
                </div>
                <div class="col-xs-4 col-sm-offset-3 col-sm-6 col-md-offset-0 text-center padding wow fadeIn" data-wow-duration="1000ms" data-wow-delay="300ms">
                    <div class="single-service">
                        <div class="wow scaleIn" data-wow-duration="500ms" data-wow-delay="300ms" height="200px">
                            <a href="{{ '/communication-skills' }}"><img src="/img/sos.jpg" title="Communication skills learningTricks of the GP trade" height="100%"></a>
                        </div>
                        <h2>Communication Skills</h2>
                        <p>Communication skills learning, tricks of the GP trade</p>
                    </div>
                </div>
                <div class="row">
                <div class="col-xs-4 col-sm-offset-3 col-sm-6 col-md-offset-0 text-center padding wow fadeIn" data-wow-duration="1000ms" data-wow-delay="900ms">
                    <div class="single-service">
                      <div class="wow scaleIn" data-wow-duration="500ms" data-wow-delay="300ms" height="200px">
                        <a href="{{ '/shared-decision-options' }}"><img src="/img/fairground.jpg" title="Swings and roundabouts, no management option suits everyone" height="100%"></a>
                        </div>
                        <h2>Shared decision options</h2>
                        <p>Swings and roundabouts, no management option suits everyone</p>
                    </div>
                </div>
                <div class="col-xs-4 col-sm-offset-3 col-sm-6 col-md-offset-0 text-center padding wow fadeIn" data-wow-duration="1000ms" data-wow-delay="900ms">
                    <div class="single-service">
                        <div class="wow scaleIn" data-wow-duration="500ms" data-wow-delay="900ms" height="200px">
                          <a href="{{ '/GP-curriculum' }}"><img src="/img/isandts.jpg" title="Dot the i’s and cross the t’s, be my apprentice" height="100%"></a>
                        </div>
                        <h2>Share our Consultations from across the GP curriculum </h2>
                        <p>Dot the i's and cross the t’s, be my apprentice</p>
                    </div>
                         </div>
                     </div>
                </div>
            </div>
    </section>

