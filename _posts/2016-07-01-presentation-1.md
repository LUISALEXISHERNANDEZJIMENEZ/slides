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

 - title: Tipos de errores
   slide-data: Al transmitir bits, la interferencia puede alterar la señal. En un error de un solo bit, un 0 cambia a 1 o viceversa. En un error en ráfaga, varios bits se alteran, por ejemplo, el ruido en una transmisión de 1200 bps podría cambiar 12 bits de información.
  
 - title: Error de un solo bit.
   slide-data: Significa que solo 1 bit de una unidad de datos (como un byte, carácter o paquete) cambia de 1 a 0 o de 0 a 1. Los errores de un solo bit son el tipo de error menos probable en la transmisión de datos en serie
  
---

{% for slide in page.slides %}
                    
<section data-background="{% if slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}"><h1>{{slide.title}}</h1>{{ slide.slide-data }}</section>
                    
{% endfor %}
    
