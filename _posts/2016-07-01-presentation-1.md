---
title: CAMBIO 2
layout: post
permalink: /presentation-1/
background: '#0a5'
slides:
 - title: cambios1
   slide-data: This is first slide
     
 - title: advwr
   slide-data: This is second slide

 - title: Slide 3
   slide-data: This is third slide
  
---

{% for slide in page.slides %}
                    
<section data-background="{% if slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}"><h1>{{slide.title}}</h1>{{ slide.slide-data }}</section>
                    
{% endfor %}
    
