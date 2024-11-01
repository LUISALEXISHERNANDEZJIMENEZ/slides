---
title: Capitulo 10
layout: post
permalink: /presentation-1/
background: '#0a5'
slides:
 - title: Deteccion y Corrección de Errores
   slide-data: 
     
 - title: Introducción
   slide-data: Para la mayoria de aplicaciones el sistema debe garantizar que los datos recibidos sean identicos a los datos transmitidos

 - title: Tipos de errores
   slide-data: Al transmitir bits, la interferencia puede alterar la señal. En un error de un solo bit, un 0 cambia a 1 o viceversa. En un error en ráfaga, varios bits se alteran, por ejemplo, el ruido en una transmisión de 1200 bps podría cambiar 12 bits de información.
  
 - title: Error de un solo bit.
   slide-data: Al transmitir bits, la interferencia puede alterar la señal. En un error de un solo bit, un 0 cambia a 1 o viceversa. En un error en ráfaga, varios bits se alteran, por ejemplo, el ruido en una transmisión de 1200 bps podría cambiar 12 bits de información.
     
 - title: Redundancia
   slide-data: Para detectar o corregir errores, se necesitan enviar bits extra junto a nuestros datos. Esta redundancia es eliminada por el receptor, permitiendo detectar o corregir los bits corruptos.

 - title: Deteccion o Correccion
   slide-data: En la detección, solo se verifica si hay un error, mientras que en la corrección se necesita saber cuántos bits están corruptos y sus ubicaciones, lo que aumenta la complejidad, especialmente en unidades de datos grandes
   
 - title: Metodos de corrección
   slide-data: Existen 2 métodos de corrección de errores; -Forward error correction; El receptor intenta adivinar el mensaje usando los bits restantes. - Retransmisión; El receptor pide al emisor reenviar el mensaje hasta que llegue sin errores. 
     
 - title: Redundancia
   slide-data: Para detectar o corregir errores, se necesitan enviar bits extra junto a nuestros datos. Esta redundancia es eliminada por el receptor, permitiendo detectar o corregir los bits corruptos.

 - title: Deteccion o Correccion
   slide-data: En la detección, solo se verifica si hay un error, mientras que en la corrección se necesita saber cuántos bits están corruptos y sus ubicaciones, lo que aumenta la complejidad, especialmente en unidades de datos grandes.

 - title: Codificar
   slide-data: El emisor añade redundancia a los bits mientras un proceso crea una relación entre los bits redundantes y los bits verdaderos detectados.
     
 - title: Aritmetica modular
   slide-data: La aritmética modular utiliza un rango limitado de enteros definido por un módulo N, que establece un límite superior. Solo se consideran los enteros del 0 al N−1. En este sistema, si un número supera N, se divide por N y se toma el residuo como resultado.Si el número es negativo, se suma N hasta que sea positivo.

 - title: Codificación por bloques
   slide-data: En la codificación por bloques, dividimos nuestro mensaje en bloques, cada uno con 'K' cantidad de bits llamada 'Palabra'. Se añaden 'r' bits redundantes para crear una longitud 'n = k + r'.

 - title: Deteccion de Errores
   slide-data: Existen maneras de detectar errores usando la codificación por bloques. - El receptor encuentra la lista de los 'Códigos' válidos. - El 'Código' original ha sido cambiado a uno inválido.

 - title: Corrección de errores
   slide-data: El receptor necesita saber que un solo 'código' es inválido. Por ello, necesita encontrar (o adivinar) el 'código' original enviado.
     
 - title: Hamming Distance
   slide-data: La Hamming distance es el número de diferencias entre sus bits. Usa un operador de XOR y cuenta el número de 1s en el resultado.

 - title: Códigos cíclicos
   slide-data: data: Los códigos cíclicos son un tipo de Código de bloques con una propiedad extra. Si un 'Código' es rotado o sus dígitos se ponen al revés, el resultado será otro 'Código' diferente.

 - title: Slide 3
   slide-data: This is thid slide 

 - title: Slide 1
   slide-data: This is first slide
     
 - title: Slide 2
   slide-data: This is second slide

 - title: Slide 18
   slide-data: This is thid slide
---

{% for slide in page.slides %}
                    
<section data-background="{% if slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}"><h1>{{slide.title}}</h1>{{ slide.slide-data }}</section>
                    
{% endfor %}
    