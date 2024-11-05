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


 - title: Medios Guiados 7.1
   slide-data: Son aquellos que proporcionan un conducto de un dispositivo a otro.
 
     
 - title: Cable de par trenzado
   slide-data: Consta de dos conductores (mayormente cobre), cada uno con su propio aislamiento plastico, trenzados entre si

   
 - title: Par trenzado blindado
   slide-data: --Tiene una lamina metalica que cubre cada par de conductores aislados. --Mejora la calidad del cable y evitar el ruido o diafonia


 - title: Categorias
   slide-data: Se determinan segun la calidad del cable, siendo 1 la mas baja y 7 la mas alta.
 
     
 - title: Conectores
   slide-data: El conector mas comun para el UTP es el RJ45. Es un conector codificado, es decir, que solo se puede insertar de una sola manera

   
 - title: Cable Coaxial
   slide-data: Consta de dos cables, tiene un conductor central de cable trenzado envuelto en una funda aislante que esta revstida por una lamina metalica. La envoltura exterior sirve para la proteccion contra el ruido .


 - title: Normas de cable coaxial
   slide-data: Se clasifican segun su clasificacion de gobierno de radio (RG). Cada cable definido por una clasificacion RG tiene una funcion especializada
 
     
 - title: Conectores de cable coaxial
   slide-data: Para conectar un cable coaxial a los dispositivos, necesitamos conectores coaxiales. El tipo de conector más común que se usa es el conector Bayone-Neill-Concelman (BNC). El conector BNC T se usa en redes Ethernet para derivar la señal a una computadora u otro dispositivo.

   
 - title: Cable de fibra óptica
   slide-data: Está hecho de vidrio o plástico y transmite señales en forma de luz. La diferencia de densidad debe ser tal que un haz de luz que se mueve a través del núcleo se refleje en el revestimiento en lugar de refractarse en él.


 - title: Modos de propagación
   slide-data: Admite dos modos (multimodo y monomodo) para propagar la luz por los canales ópticos, cada uno requiere fibras con características físicas diferentes. El modo multimodo se puede implementar en dos formas; índice escalonado o índice graduado.

   
 - title: Multimodo
   slide-data: Varios haces de una fuente de luz se mueven a través del núcleo en diferentes trayectorias. La forma en que estos haces se mueven dentro del cable depende de la estructura del núcleo


 - title: Slide 1
   slide-data: This is first slide
 
     
 - title: Slide 2
   slide-data: This is second slide

   
 - title: DS
   slide-data: This is third slide

 - title: IP
   slide-data: This is third slide


 - title: Slide 2
   slide-data: This is second slide

   
 - title: Slide 3
   slide-data: This is third slide


 - title: Slide 1
   slide-data: This is first slide
 
     
 - title: Slide 2
   slide-data: This is second slide

   
 - title: AH
   slide-data: This is third slide

---

{% for slide in page.slides %}
                    
<section data-background="{% if slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}"><h1>{{slide.title}}</h1>{{ slide.slide-data }}</section>
                    
{% endfor %}
    
