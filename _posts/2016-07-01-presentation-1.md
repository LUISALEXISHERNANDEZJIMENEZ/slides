---
title: CAPITULO 10
layout: post
permalink: /presentation-1/
background: '#0a5'
slides:
 - title: Deteccion y Corrección de Errores 
   slide-data: 
     
 - title: 
   slide-data: Para la mayoria de aplicaciones el sistema debe garantizar que los datos recibidos sean identicos a los datos transmitidos

 - title: Slide 3
   slide-data: This is third slide
  
---

{% for slide in page.slides %}
                    
<section data-background="{% if slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}"><h1>{{slide.title}}</h1>{{ slide.slide-data }}</section>
                    
{% endfor %}
    
