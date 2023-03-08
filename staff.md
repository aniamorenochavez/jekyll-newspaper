--
layout: makeup yaret

title: makeup


# {{ la belleza interios de yaret moreno)

<h3 style="text-align: justify;"> A MI DISDE MUY CHICA  ME AH GUSTADO MUCHO TANTO QUE ASI DISDE ,UY CHICA EJ JUGADO CON EL MAQUILLJE  EH TENIDO MUVHO MAQUILLAJE TANTO ASI Q HASTA EL DIA DE HOY  TEMGO UN BUEN Y ME GUSTA MUCHO COMO ME MAQUILLO  COMO YO QUIERO  AL IGUAL QUE LAS PESTANAS  EMTPCES SIEMPRE QUE ME MAQUILLO ME GUSTA ARRGLARME PARA VERME LIMPIA Y FRESCA Y RADIANTE 

<h1>&nbsp;</h1>
{% for author in site.authors %}

<div class="row">

  <div class="col col-8 rounded"  
       style="
         background-color: #eeefff;
         padding: 22px;
         box-shadow: 
           inset 0 3em 3em rgba(0, 0, 0, 0.1), 
                 0 0 0 -2px rgb(255, 255, 255), 
                 0.3em 0.3em 1em rgba(0, 0, 0, 0.3); 
  ">
    <div class="row"> 
      <div class="col-4">
        <h3>{{author.name}}</h3>ANIA YARET MORENO CHAVEZ 
        <img class="img-fluid" src="{{site.url}}{{site.baseurl}}{{author.profile_img}}" />
        <p></p>
        <h5></h5>
        <p><strong>Email:</strong><br/>{{author.email}}</p> morenochavezyaret157@gmail.com
        <p><strong>Phone:</strong><br/>{{author.phone}}</p>5587792586
        <p><strong>Location:</strong><br/>{{author.location}}</p>vivo en la segunda avenida numero  71 colonia el sol nezahualcoyolt  codigo postal  57200
        <div class="d-grid gap-2">
          <a href="{{site.url}}{{site.baseurl}}/authors/{{ author.github }}" class="btn btn-block btn-outline-primary" >
            Visit Author Page</a> 
        </div>
      </div>
      <div class="col-8">
        <h3>Staff Bio</h3>
        <article style="text-align: justify;">
          {{ author.excerpt }}
        </article>
        <h5><strong>{{author.position}}, {{author.name}}</strong></h5> mi bibliografia de YARET MORENO CHAVEZ
        NACI EN LA CUIDAD DE MEXICO EL 21 DE FEBREO DEL 2004  CASI A LAS 8PM DE LA NOCHE  MIS PAPAS SE LLAMAN ROSALBA CHAVEZ VAZQUEZ  Y MI PAPA SE LLAMA JUAN CRISOFORO MORENO MENDOZA   Y MI HERMANO SE LLAMA JUAN  ARMANDO MORENO CHAVEZ  ESTUDI EN EL KINDER A LOS 5 ANOS DE EDAD JUNTO CON MIES MEJORES AMIGAS ABRIL ITZEL, ITZEL MARITZA , LLUVIA HERNANDEZ Y SANDRA ESTUDIE AHI COMO  A LOS 4 ANOS DE AHI ESAS AMISTADES 15 ANOS DE AMISTAD AUNQUE POR MOTIVOS PERSONALES LES DEJE DE HABLAR SOLO AUNA LE HABLO   A MI AMIGA ABRIL  ITZEL   PUES EN LA RPIMARIA DISDE PRIMERO HASTA SEXTO  CON MUY BUENOS PROFESORES  AHI CONOCI A LA MAYORIA DE MIS AMISTADES AUNQUE AGUNAS PERDI HUELLA DE ELLAS PERO AHI SIGO  ME LA PASABA SUPER BIEN AUNQUE COMO NO SOY BUENA EN MATEMATICCAS PUES  ME REGANABAN UN POCO MAS DE LO DEBIDO JAJAJ PERO BUENO ASI PASABA LOS GRADOS DE LAS PRIMARIA PARA  LA GRADUACION  Y DESPUES PASE A LA SECUNDARIAS SECUNDARIA TECNICA NUMERO 69 CESAR USCANGA USCANGA  DONDE ESTUDIE TRES 3 ANOS Y LOS MJORES EH FASTIDIOSOS DE MI VIDA POR QUE PUES ESTABA CAMBIQNDO AUNQUE NO ESTABA TAN BONITA AUN ASI TRAIA MI PAGUE OUES SUFRI MUCHO POR QUE ME HACIAN BULLING POR NOA RREGLARME 
        <hr> 
        <h3>Articles by this author</h3>
        {% for post in site.posts %}
          {% if post.author == author.github %}
            <p><a href="{{site.url}}{{site.baseurl}}{{ post.url }}"><strong>{{ post.title }}</strong></a> - By: {{post.author}}</p>
          {% endif %}
        {% endfor %}
      </div>
    </div>
{% endfor %}
    
  </div>
  <div class="col col-4 bg-old-paper rounded">
    {% include about_section.html %} 
    {% include social_links.html %}
    {% include archives_section.html %}
    {% include pages_section.html %}
    {% include tag_cloud.html %}
  </div>

</div>
