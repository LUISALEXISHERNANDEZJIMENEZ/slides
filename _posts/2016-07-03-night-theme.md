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


 - title: Slide 1
   slide-data: This is first slide
 
     
 - title: Normas de cable coaxial
  slide-data: Se clasifican según su clasificación de gobierno de radio (RG). Cada cable definido por una clasificación RG tiene una función especializada.

- title: Conectores de cable coaxial
  slide-data: Para conectar un cable coaxial a los dispositivos, necesitamos conectores coaxiales. El tipo de conector más común que se usa es el conector Bayone-Neill-Concelman (BNC). El conector BNC T se usa en redes Ethernet para derivar la señal a una computadora u otro dispositivo.

- title: Cable de fibra óptica
  slide-data: Está hecho de vidrio o plástico y transmite señales en forma de luz. La diferencia de densidad debe ser tal que un haz de luz que se mueve a través del núcleo se refleje en el revestimiento en lugar de refractarse en él.

- title: Modos de propagación
  slide-data: Admite dos modos (multimodo y monomodo) para propagar la luz por los canales ópticos, cada uno requiere fibras con características físicas diferentes. El modo multimodo se puede implementar en dos formas; índice escalonado o índice graduado.

- title: Multimodo
  slide-data: Varios haces de una fuente de luz se mueven a través del núcleo en diferentes trayectorias. La forma en que estos haces se mueven dentro del cable depende de la estructura del núcleo.

- title: Multimodo índice graduado
  slide-data: Es una fibra con densidades variables. La densidad es más alta en el centro del núcleo y disminuye gradualmente hasta su nivel más bajo en el borde.

- title: Monomodo
  slide-data: Utiliza fibra de índice escalonado y una fuente de luz enfocada que limita los haces a un pequeño rango de ángulos. La disminución de la densidad da como resultado un ángulo crítico que está lo suficientemente cerca de 90° para hacer que la propagación de los haces sea casi horizontal.

- title: Tamaños de fibra
  slide-data: Se definen por la relación entre el diámetro de su núcleo y el diámetro de su revestimiento, ambos expresados ​​en micrómetros.

- title: Composición de cables
  slide-data: La cubierta exterior está hecha de PVC o teflón. En el interior de la cubierta hay hilos de Kevlar para reforzar el cable. Debajo del Kevlar hay otro revestimiento de plástico para amortiguar la fibra. La fibra está en el centro del cable y consta de revestimiento y núcleo.

- title: Conectores de cable de fibra óptica
  slide-data: Existen varios tipos de conectores diseñados para cables de fibra óptica, adaptados para aplicaciones específicas.


- title: Medios no guiados: inalámbrico
  slide-data: Transportan ondas electromagnéticas sin utilizar un conductor físico. Este tipo de comunicación se conoce a menudo como comunicación inalámbrica. Las señales se transmiten a través del espacio libre y están disponibles para cualquier persona que tenga un dispositivo capaz de recibirlas.

- title: Bandas
  slide-data: Las ondas de radio y microondas se dividen en ocho rangos, denominados bandas. Estas bandas se clasifican desde frecuencias muy bajas (VLF) hasta frecuencias extremadamente altas (EHF).

- title: Ondas de radio
  slide-data: Las ondas de radio, en su mayor parte, son omnidireccionales. Cuando una antena transmite ondas de radio, estas se propagan en todas las direcciones. Las ondas de radio, en particular las que se propagan en el cielo, pueden viajar grandes distancias. El uso de cualquier parte de la banda requiere el permiso de las autoridades.

- title: Microondas
  slide-data: Las ondas electromagnéticas que tienen frecuencias entre 1 y 300 GHz se denominan microondas. Las microondas son unidireccionales, y su propagación se produce en línea de visión. Las microondas de muy alta frecuencia no pueden atravesar paredes. La banda es relativamente amplia, casi 299 GHz. El uso de ciertas partes de la banda requiere permiso de las autoridades.

- title: Antena unidireccional.
  slide-data: Las microondas necesitan antenas unidireccionales que envíen señales en una dirección. Para las comunicaciones por microondas se utilizan dos tipos de antenas; la antena parabólica y la antena de bocina.

- title: Infrarrojo
  slide-data: Las ondas infrarrojas, con frecuencias de 300 GHz a 400 THz (longitudes de onda de 1 mm a 770 nm), se pueden usar para la comunicación de corto alcance. Las ondas infrarrojas, que tienen frecuencias altas, no pueden atravesar paredes.

- title: Gracias
  slide-data: Agradecemos su atención.


---

{% for slide in page.slides %}
                    
<section data-background="{% if slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}"><h1>{{slide.title}}</h1>{{ slide.slide-data }}</section>
                    
{% endfor %}
    
