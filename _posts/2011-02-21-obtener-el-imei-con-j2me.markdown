---
title: "Obtener el IMEI con J2ME"
layout: post
date: 2011-02-21 00:04:38.000000000 -03:00
category: blog
tag: J2ME
star: true
author:Yury Camacho
description: Obtener el IMEI con J2ME
---

<p>Desde hace tiempo andaba buscando por la web la forma de obtener al IMEI de un movil atravez de J2ME y  despues de ver algunos lugares ( por no decir ........ perder el tiempo leyendo varios  blogs que no tenian  una buena informacion ).<br />
encontre una respuesta en <a rel="nofollow" href="http://wiki.forum.nokia.com /index.php/How_to_get_IMEI_in_Java_ME">esta pagina</a>, ojo que esta en ingles..y para los que les da flojera traducir aqui le dejo una pequeña explicacion de esto:para nuestra mala suerte  no hay una forma  standar de conseguir el  imei, ademas no en todos los dispositivos es posible obtener el numero de imei  ,  es depende del fabricante  de dispositivo, veamos el codigo para  algunos dispositivos:</p>
<ul>
<li> <strong>Siemens:</strong> System.getProperty("com.siemens.IMEI");</li>
<li> <strong>Samsung: </strong>System.getProperty("com.samsung.imei");</li>
<li> <strong>SonyEricsson:</strong> System.getProperty("com.sonyericsson.imei");</li>
<li> <strong>Motorola: </strong>System.getProperty("IMEI");    ó  System.getProperty("com.motorola.IMEI");</li>
<li> <strong>Nokia: </strong>System.getProperty("com.nokia.mid.imei")</li>
</ul>
<p>yo tuve la oportunidad de probarlo en dos marcas:  nokia (5800) y  sonny ericsson(w760i) , todo salio bien :) obtuve los respectivos IMEI's</p>
<p>si alguien lo prueba con otras marcas comenten contando como les fue ...</p>

