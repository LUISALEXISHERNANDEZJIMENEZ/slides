---
title: Capitulo 7
layout: post
permalink: /night/
theme: night
 
slides:
 - title: Capitulo 7
   slide-data: --Hernandez Jimenez Luis Alexis
 
     
 - title: Medios de Transmisión
   slide-data: Un medio de transmision puede definirse como cualquier cosa que puede llevar informacion desde una fuente a un destino

   
 - title: 
   slide-data: Se pueden dividir en dos grandes categorias; --Guiados; Incluyen el par trenzado, cable coaxial y cable de fibra optica  --No guiados; Es el espacio libre


 - title: Slide 1
   slide-data: This is first slide
 
     
 - title: Slide 2
   slide-data: This is second slide

   
 - title: Slide 3
   slide-data: This is third slide


 - title: Capitulo 7
   slide-data: This is first slide
 
     
 - title: Slide 2
   slide-data: This is second slide

   
 - title: Slide 3
   slide-data: This is third slide


 - title: Slide 1
   slide-data: This is first slide
 
     
 - title: Slide 2
   slide-data: This is second slide

   
 - title: IP
   slide-data: This is third slide

---

{% for slide in page.slides %}
                    
<section data-background="{% if slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}"><h1>{{slide.title}}</h1>{{ slide.slide-data }}</section>
                    
{% endfor %}
    
