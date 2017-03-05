---
title: Verificar si un punto esta dentro de un poligono en postgis
layout: post
date: 2012-08-21 10:03:43.000000000 -03:00
headerImage: false
category: blog
tag: 
    - Posgis
    - Postgres
author: camachoyury
description: Verificar si un punto esta dentro de un poligono en postgis
  
---
<p>Si Postgis no existiera esto seria un poco complicado,  ok.. la tarea es la siguiente en mi base de datos tengo unas cercas que no son mas que unos poligonos, y necesitaba saber si el punto que lanzaba desde un gps al sevidor  esta dentro de el poligono o fuera, Postgis nos da una funcion llamanda <a title="ST_Contains" href="http://postgis.refractions.net/documentation/manual-1.4/ST_Contains.html" target="_blank">ST_CONTAINS</a>  que nos permite ver si un punto esta dentro de un poligono, esta funcion recibe dos parametros que son del tipo GEOMETRY :</p>
<p>ST_CONTAINS(geometry, geometry)</p>
<p>el primer parametro es el poligono y el segundo es el punto. y listo ya sabemos si el punto esta dentro del poligono, ok ahora tengo un ejemplo el cual es una funcion que  solo verifica si el punto enviado esta dentro de una geocerca ya almacenada en la base de datos (ojo que es un ejemplo hardcode) ya ustedes lo pueden modificar de acuerdo  a lo que necesitan:</p>
<p><code><br />
CREATE OR REPLACE FUNCTION in_polygon()<br />
<strong>-- retorna un booleano true si esta dentro y false si esta fuera</strong><br />
RETURNS boolean AS<br />
$$<br />
DECLARE<br />
<strong>--se declara una variable que almacenara el poligono que se sacara de la base de datos</strong><br />
v_geom geometry;<br />
<strong>-- la variable de respuesta</strong><br />
v_result BOOLEAN ;<br />
BEGIN<br />
<strong>-- se saca el poligono de la tabla geofence</strong><br />
v_geom := (SELECT geo.geom from geofence as geo where id_geofence = 18);<br />
<strong>--y se usa la funcion de postgis</strong><br />
v_result := (SELECT ST_Contains(v_geom, GeomFromText('POINT(-65.9667 -17.474)',4326)));<br />
RETURN v_result;<br />
END;<br />
$$<br />
LANGUAGE plpgsql VOLATILE<br />
</code></p>
<p>ya ustedes pueden aumentar parametros a la funcion , condiciones, ect.</p>
<p>espero que les sirva</p>
