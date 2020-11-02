# BorjaPavonWad

## 0. Versiones y cambios

    02/11/2020:
    Mejorado el volumen en algunos sonidos. Añadidos sonidos para las opciones "Spacial Chocolation" y otros.
    Este fichero NO incluye cambios en las imágenes del Doom. Esto solo incluye cambios en los sonidos. Los archivos para cambiar texturas y enemigos, por el momento NO los voy a compartir por tema de copyright y por si alguien se siente ofendido (Borja Pavon, Hideo Kojim,a Steven Seagal :-) )
    25/10/2020:
        Comienzo de FAQ... y próximo proyecto...

    10/10/2020:   
    Añadidos dos efectos nuevos. No son gran cosa pero bueno. Para verlos rapidamente lo mejor es ir al nivel map20 (idclev20) y luchar contra arañas (grande y pequeña) y el Cyberdemonio

    Cambios en documentacion menores. Comando para probar sonidos desde la consola
              
## 1. Introducción

### 1.1. ¿Qué es esto?
El videojuego Doom ([el antiguo, el de 1993](https://es.wikipedia.org/wiki/Doom_(videojuego_de_1993))) permite añadirle ficheros (WAD o PK3) con modificaciones (mods) que pueden incluir nuevos niveles, armas o imágenes y sonidos.
Por ejemplo, están el [Chiquito de laCalzada.wad](https://www.youtube.com/watch?v=WZnbjulJNCw) y varios [Simpsons.wad](https://www.youtube.com/watch?v=6ZLN4WOS1Ts) .

Con esta idea, he creado un fichero WAD (bueno, técnicamente es un archivo .pk3, pero es casi lo mismo) que reemplaza algunos de los sonidos originales por voces y efectos de [Borja Pavon](https://twitter.com/kidcoltrane)

### 1.2 ¿Qué NO es esto?

No se modifican los gráficos ni los niveles. Sólo los efectos del sonido. No es un juego independiente, se necesita una versión del Doom existente para jugar.

## 2. Instalación 

### 2.1 Instalación del Doom original (paso previo imprescindible)

Primero descargar algun "engine" moderno compatible con Doom. Yo he probado y sugiero el gzdoom.
Ir a https://zdoom.org/downloads y descargar el GZDoom v4.4.2 

Se descarga como un archivo .zip, así que hay que descomprimirlo en alguna carpeta nueva aparte para él, como por ejemplo C:\gzdoom.
Si intentamos arrancar el programa, haciendo doble click en el ejecutable gzdoom.exe, saldrá mensaje de error indicando que necesita los archivos de datos originales del juego.

Una búsqueda en google debería devolvernos los archivos .WAD que necesitamos. Por ejemplo https://pc-freak.net/blog/doom-1-doom-2-doom-3-game-wad-files-for-download-playing-doom-on-debian-linux-via-freedoom-open-source-doom-engine/.

Descargar el doom2.wad. El doom1.wad incluido en la web anterior es la versión Shareware , y además no se si será compatible con los cambios que he hecho.
Colocar el doom2.wad en el mismo directorio que gzdoom, en C:\gzdoom por ejemplo.

Si ahora abrimos el ejecutable ya debería funcionar y podremos jugar.

Echate unas partidas, configura las teclas, el volumen (*recomiendo bajar el volumen de la música al mínimo*) y todo al gusto de cada uno. 
Y recordar [los trucos habituales de Doom](https://doom.fandom.com/wiki/Doom_cheat_codes):

idclip  (atravesar paredes)

iddqd  (invulnerabilidad)

idkfa   (todas las armas y llaves)

idclev##  (ir al mapa ##)


**No pasar al siguiente punto hasta que no funcione lo anterior.**

### 2.2 Instalación del Wad (bueno, pero da igual, es un .pk3)

Descarga el archivo BorjaPavonWad.pk3 (entra dentro de el arriba y luego pulsa Download, o usa este enlace directo https://github.com/basuradeluis/BorjaPavonWad2/raw/master/BorjaPavon.pk3) y colócalo de la misma manera que el doom2.wad dentro de C:\gzdoom.

**No es necesario descargar nada más**

Para cargar el fichero .pk3 con el Doom, arrastra con el ratón el fichero .pk3 al ejecutable  gzdoom.exe. De esta forma se abrirá el juego con la modificación. Seguramente hay otras maneras distintas de hacerlo, pero involucran cambiar archivos .ini.

Échate unas partidas. Muevete por los menús. Intenta abrir puertas, y plataformas. Haz un sandwich de explosiones con los barriles y el lanzacohetes. Finaliza al menos un nivel. Déjate matar, etc.

Por cierto los archivos .pk3 son en realidad archivos .zip, que se pueden abrir con cualquier aplicación que los abra, como el Winrar, 7Fm Zip file  y puede que el explorador de archivos de windows si se configura adecuadamente. Échale un vistazo, si tienes curiosidad. Está formado por archivos de sonido (son archivos .wav sin extensión, para ahorrar letras) y un archivo txt de configuración donde está la configuración de los sonidos y los eventos que los lanzan.


## 3. Extra

### 3.1 Making of
Usé una web cualquiera que transforma videos de youtube a mp3 (https://ytmp3.cc/en13/).

Luego con el AudaCity recorté los sonidos y los pasé a .WAV. 

Y finalmente usé la herramienta de modificacion de Doom [Slade](https://slade.mancubus.net/) para configurar sonidos y eventos del juego (*)

No encontré tutoriales muy claros para modificar los sonidos del juego así que he tenido que aprender un poco a base prueba y error. Pero estas web me ayudaron:

http://gunlabs.blogspot.com/2011/03/tutorial-adding-your-own-sound-effects.html

http://gunlabs.blogspot.com/2011/01/tutorials.html

https://www.reddit.com/r/Doom/comments/6jb76j/i_want_to_start_making_doom_wads/

https://github.com/rheit/zdoom/blob/master/wadsrc/static/filter/game-doomchex/sndinfo.txt

http://slade.mancubus.net/index.php?page=wiki&wikipage=Supported-Data-Formats

https://zdoom.org/wiki/SNDINFO

(*) Aunque estoy pensando que prácticamente se podia haber hecho todo con un simple editor de texto y un programa para editar archivos .zip


Para probar los efectos de sonido -aunque asi pierde toda la gracia de la sorpresa- , se puede abrir la consola (tecla "ºª\\") y luego teclear comandos como 

playsound spider/active

playsound misc/secret

playsound pl_death

Algunos sonidos se reproducen de manera aleatoria por cada evento, asi que hay que darle a reproducir varias veces cada evento. Con la tecla cursor arriba se repite el mismo comando anterior tecleado y es más facil.

### 3.2 Fuentes
[Death Strundun - Making of con Hideo Kojima (Borja Pavón)](https://www.youtube.com/watch?v=Hx1Qzb3-yag)

[Entrevista en profundidad: Hideo Kojima (PARODIA) (Borja Pavón)](https://www.youtube.com/watch?v=jYYPtJW8J9M)

[La vida en Animal Crossing #2 (Borja Pavón)](https://www.youtube.com/watch?v=QPwh1WHDeBU)

Actualización 10/10/2020:

[5 JUEGOS CANCELADOS que tampoco ECHAMOS DE MENOS](https://www.youtube.com/watch?v=8te9-s5G_Kc)

[Los MOMENTOS MÁS LOCOS de los VIDEOJUEGOS #5](https://www.youtube.com/watch?v=NV24t8rSogY)

### 3.3 Copyright
Dez Strundun es una marca de Borja Pavón. 
Chonfluns también. 
Hideo Kojima es una marca registrada de sí mismo.
Etc, etc etc :-)
Doom es una marca registrada de idSoftware

### 3.4 Disclaimer:
Es mi primer (y último seguramente) modificación al Doom. No soy ningún experto pero bueno. Seguro que se puede hacer mejor o más divertido. Adelante, hazlo tú.

### 3.5 FAQ:
25/10/2020:
"¿Se podrían cambiar además de los sonidos, las imagenes del Doom para poner, por ejemplo a Chonfluns, a Tom Nook, a Borja en las paredes y como enemigos?:
Si, en teoría se puede hacer. Pero no quedaría bien porque no soy diseñador gráfico ni se nada de eso. Además cuesta mucho: está mal documentado/explicado en internet.... A no ser que.... Misterio"
