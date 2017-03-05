---
title: "Instalando Eclipse y Android SDK"
layout: post
date: 2012-08-02 22:02:44.000000000 -03:00
category: blog
tag:
- eclipse
- google
- Android
meta:
  tagazine-media: a:7:{s:7:"primary";s:61:"http://camachoyury.files.wordpress.com/2012/07/adt-plugin.jpg";s:6:"images";a:5:{s:65:"http://camachoyury.files.wordpress.com/2012/07/installnewsw11.jpg";a:6:{s:8:"file_url";s:65:"http://camachoyury.files.wordpress.com/2012/07/installnewsw11.jpg";s:5:"width";i:807;s:6:"height";i:382;s:4:"type";s:5:"image";s:4:"area";i:308274;s:9:"file_path";b:0;}s:61:"http://camachoyury.files.wordpress.com/2012/07/adt-plugin.jpg";a:6:{s:8:"file_url";s:61:"http://camachoyury.files.wordpress.com/2012/07/adt-plugin.jpg";s:5:"width";i:776;s:6:"height";i:641;s:4:"type";s:5:"image";s:4:"area";i:497416;s:9:"file_path";b:0;}s:60:"http://camachoyury.files.wordpress.com/2012/07/dev-tool1.jpg";a:6:{s:8:"file_url";s:60:"http://camachoyury.files.wordpress.com/2012/07/dev-tool1.jpg";s:5:"width";i:736;s:6:"height";i:633;s:4:"type";s:5:"image";s:4:"area";i:465888;s:9:"file_path";b:0;}s:58:"http://camachoyury.files.wordpress.com/2012/07/sdk-dw1.jpg";a:6:{s:8:"file_url";s:58:"http://camachoyury.files.wordpress.com/2012/07/sdk-dw1.jpg";s:5:"width";i:619;s:6:"height";i:464;s:4:"type";s:5:"image";s:4:"area";i:287216;s:9:"file_path";b:0;}s:65:"http://camachoyury.files.wordpress.com/2012/07/androidtools11.jpg";a:6:{s:8:"file_url";s:65:"http://camachoyury.files.wordpress.com/2012/07/androidtools11.jpg";s:5:"width";i:213;s:6:"height";i:55;s:4:"type";s:5:"image";s:4:"area";i:11715;s:9:"file_path";b:0;}}s:6:"videos";a:0:{}s:11:"image_count";i:5;s:6:"author";s:8:"19738260";s:7:"blog_id";s:8:"19140729";s:9:"mod_stamp";s:19:"2012-08-03
    02:32:44";}
  _edit_last: '19738260'
  _oembed_0af63133e281556dbd843369e3fdfe8e: "{{unknown}}"
  _oembed_b3977bcc2654a52255b3f2cd1f74c037: "{{unknown}}"
  _oembed_933afbc7215d50aabfb629c23af82ec7: "{{unknown}}"
  _oembed_5b436854ba39bd934de197b4d46e7cef: "{{unknown}}"

author: camachoyury
description: Instalando Eclipse y Android SDK
---
<p>Hace un tiempo que ando metido en esto de android..y decidí hacer una serie de post para quienes están iniciando en este maravilloso mundo.. Al empezar a desarrollar sobre cualquier tecnología siempre  es un poco complicado entender algunas cosas, pero gracias  a San Google y el internet todo resulta mas fácil, en internet existen muchos tutoriales de como instalar o configurar nuestro propio entorno de desarrollo para programar aplicaciones Android, y siempre  es mejor que sobre a que falte, por eso decidi realizar un tutorial  de como configurar nuestro entorno de desarrollo para Android.</p>
<p>Nota: el tutorial esta bajo  el sistema operativo Windows 7..pese que yo utilizo una mac  ;)</p>
<p><strong>MANOS A LA OBRA</strong></p>
<p>1. - Primero que nada tenemos que tener instalado java en nuestra maquina. me salto este paso por que no es el motivo     principal del tutoria.. en internet existen muchos  tutoriales acerca del tema.</p>
<p>2.-   Descargarnos el IDE Eclipse, lo hacemos desde el siguiente link :  <a title="Eclipse" href="http://www.eclipse.org/downloads/" target="_blank">Eclipse</a>.</p>
<p>3.- Descargamos el Android SDK del siguiente link: <a title="Android SDK" href="http://developer.android.com/sdk/index.html" target="_blank">Android SDK</a>.</p>
<p>4.- Ok, Ahora solo resta instalar y configurar nuestro entorno!!!</p>
<p>Para poder desarrollar en eclipse  es necesario instalarnos el plugin de android (Android ADT),En Eclipse tenemos que dirigirnos  a Help&gt;Install New Software,  como se ve a continuación:</p>
<p><a href="http://camachoyury.files.wordpress.com/2012/07/installnewsw11.jpg"><img class="aligncenter size-full wp-image-260" title="installNewSW1" src="{{ site.baseurl }}/assets/installnewsw11.jpg" alt="" width="620" height="293" /></a></p>
<p>posteriormente se mostrara una ventana donde se agragano actualizan los plugnis instalados en eclipse,  en el cual se vera el botón con el nombre  "Add", le damos click en el botón y se abrira una ventana donde se agrega la URL de donde se descargara el ADT como se ve  a continuación:</p>
<p><a href="http://camachoyury.files.wordpress.com/2012/07/adt-plugin.jpg"><img class="aligncenter size-full wp-image-262" title="ADT-plugin" src="{{ site.baseurl }}/assets/adt-plugin.jpg" alt="" width="620" height="512" /></a></p>
<p>en el campo "Name"  podemos poner cualquier nombre..en mi caso puse un nombre que identifiqur al plugin "ADT - plugin", en el campo "Location"  escribimos la url de donde se descargara el plugin, tenemos dos opciones:</p>
<ul>
<li><em>https://dl-ssl.google.com/android/eclipse/</em></li>
<li><em>http://dl-ssl.google.com/android/eclipse/</em></li>
</ul>
<p>Recomiendo la segunda URL para no tener problemas.</p>
<p>Después  de agregar la URL  se mostara la lista de plugins en el cual seleccionamos la primera opcion (Developer Tools),  la segunda opcion es el plugin de android para desarrollar aplicaciones escritas en C/C++.</p>
<p><a href="http://camachoyury.files.wordpress.com/2012/07/dev-tool1.jpg"><img class="aligncenter size-full wp-image-263" title="dev tool1" src="{{ site.baseurl }}/assets/dev-tool1.jpg" alt="" width="620" height="533" /></a></p>
<p>luego aceptamos la licencia..y nos vamos a tomar un café mientras instala el plugin, nos pedira reiniciar eclipse lo reiniciamos y luego de reiniciarlo nos saldra uan ventana como se muestra a continuacion, donde nos pide la direccion de nuestro Android SDK.</p>
<p><a href="http://camachoyury.files.wordpress.com/2012/07/sdk-dw1.jpg"><img class="aligncenter size-full wp-image-264" title="sdk dw1" src="{{ site.baseurl }}/assets/sdk-dw1.jpg" alt="" width="619" height="464" /></a></p>
<p>Aca tenemos dos opciones, una es la primera la cual nos descargara el Android SDK, pero como nosotros nos descargamos el sdk de android lo que hacemos es descomprimir en cualquier directorio o instalar si te bajaste el .exe , seleccionar la segunda opcion "Use existing SDKs", y le damos la ruta donde descomprimimos el Android SDK.</p>
<p>una ves ya instalado de manera correcta nuestro entorno en la barra superior veremos los dos botones que se muestran a continuación:</p>
<p><a href="http://camachoyury.files.wordpress.com/2012/07/androidtools11.jpg"><img class="aligncenter size-full wp-image-266" title="androidtools1" src="{{ site.baseurl }}/assets/androidtools11.jpg" alt="" width="213" height="55" /></a></p>
<p>El icono de la izquierda(rojo) es el botón que nos abre el SDK Manager con el cual nos descargamos las apis de android, y el de la derecha (Azul) abre el Android Virtual Device Manager.... en el cual podemos crearnos dispositivos virtuales para probar nuestras aplicaciones.</p>
<p>Espero que les sirva este post...si lo usaron no se olviden comentar....</p>
