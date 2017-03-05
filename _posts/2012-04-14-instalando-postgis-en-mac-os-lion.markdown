---
layout: post
title: Instalando Postgis en Mac OS Lion
date: 2012-04-14 13:39:49.000000000 -03:00

category: blog
tags: 
- postgres
- postgis
- MacOS
meta:
  _edit_last: '19738260'
author: Yury Camacho
description: Instalando Postgis en MacOSX Lion
  
---
<p>Hace unas semanas adquiri una nueva computadora, es una MacBook Pro, que se las recomiendo mucho a todos si es que trabajan con tecnologias libres mejor dicho con tecnologias que no son Windows (Java, PHP, Python, etc.), aunque ahora si se puede tener instalado Windows en una Mac, pero es un poco ridiculo adquirir una Mac y ponerle Windows, el caso es que me puse la tarea de instalarle todo lo que un developer necesita (Postgres), y como dice el titulo de este post quize instalar postgis en mac os, pero fue grande la sorpresa!!!.... descargue el instalador de postgres 9.1 para mac despues de instalarlo inicie la aplicacion Application Stack Builder seleccione postgis 1.5, pero despues de descargar el instalador este no se ejecutaba..como en algun momento vi que lo hacia bajo Windows 7.</p>
<p>Entonces despues de navegar, leer un monton de posts y articulos, encontre la solucion:</p>
<p>Primero que nada es un bug de Stack Builder el hecho de que no se instale, la soluion es sencilla: tenemos que ubicar donde es que stack builder descaro el instalador para hacer correr de manera manual por consola(Terminal) y con permisos de super usuario que si no, no se podra ver lo que esta dentro la carpeta "T" , en mi caso estaba en:</p>
<p><code> /var/folders/gz/jx9m7c211hjgzn51vv9zxjgm0000gm/T/<br />
</code></p>
<p>Ahi encontraran el .zip de postgis que es : edb_postgis_1_5_pg91.app.zip , una vez ubicado, la siguiente tarea es la de descomprimir con el comando:</p>
<p><code> unzip edb_postgis_1_5_pg91.app.zip </code><br />
y esto descomprimira un .app postgis-pg91-1.5.3-1-osx.app el siguiente paso es ejecutar el instalador con el comando:<code><br />
open postgis-pg91-1.5.3-1-osx.app/<br />
</code></p>
<p>ok, y listo tendremos instalado postgis 1.5 en Mac OS Lion.</p>
