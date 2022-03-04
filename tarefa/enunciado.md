
## Ej1. LAYOUT FLUIDO (**2 pts**)

Modificar el fichero CSS ‘01-layout-fluido/01-layout-fluido.css’ para que la página HTML ‘01-layout-fluido/01-layout-fluido.html’
se visione de la siguiente forma:
   - La capa azul siempre está a la izquierda de la capa roja.
   - La capa azul tiene que ocupar el 70% mientras que la capa roja el 30%
   - El texto de la capa azul es el doble de grande que el de la capa roja.
   - Que la suma de las dos capas (la azul y la roja) no supera nunca los 1024 píxeles.
	
En la carpeta del ejercicio dispones de 3 imágenes de ejemplo de cómo se debe visualizar la pagina para 3 resoluciones de pantalla distintas (los valores son meramente orientativos)


## Ej2. DESKTOP FIRST (**2 pts**)

Modificar el fichero CSS ‘02-desktop-first/02-desktop-first.css’ para que la página HTML ‘02-desktop-first/02-desktop-first.html’
se visione de la siguiente forma:
   - La imagen de fondo de la capa azul va cambiando dependiendo del tamaño del dispositivo. La primera imagen que se carga es la más grande, para los dispositivos más grandes.
   - En dispositivos pequeños el ‘sidebar’ se posiciona debajo ocupando el 100% y en dispositivos medianos y grandes se posiciona a la derecha ocupando el 30%.
   - Breakpoints:
		- Dispositivos medianos: 880px
		- Dispositivos pequeños: 580px
En la carpeta del ejercicio dispones de 3 imágenes de ejemplo de cómo se debe visualizar la pagina para dispositivos grandes, medianos y pequeños.



## Ej3. IMAGENES RESPONSIVE (**4 pts**)

Crea un documento HTML  que cumpla con las siguientes especificaciones:
   - Usar etiquetas semánticas HTML5 que sean necesarias.
   - El título de la página debe ser “Praza do Obradoiro”
   - El cuerpo de la página debe ter una anchura variable hasta un máximo de 1000px.
   - La cabecera debe ocupar todo el ancho del body con 200px de alto, con una imagen de fondo.
		- Puedes escoger cualquiera con dimensiones mínimas de 1000px x 200px pero sería recomendable que crees una imagen exactamente de esas dimensiones, para non desperdiciar ancho de banda cargando una image muy grande.
   - Deberá tener un menú de navegación con tres elementos:
		- “Inicio”
		- “Concello de Santiago” con un enlace a un artículo del mismo título dentro de esta misma página.
		- “Catedral de Santiago” con un enlace a un artículo del mismo título dentro de esta misma página.
   - El contenido principal de la página serán los artículos anteriores:
		- “Concello de Santiago” que tendrá un título con este nombre, un texto, y una imagen con el logotipo del concello de Santiago, con 200px de ancho. Al pulsar sobre el logo nos lleva a la web del concello de Santiago: http://santiagodecompostela.gal/
		- “Catedral de Santiago” que tendrá un título con este nombre, un texto, y una imagen de la catedral de Santiago que variará según la anchura de la ventana de navegación empleando la etiqueta `<img>` y los atributos srcset y sizes. A continuación, más texto, y por último otra imagen de la catedral de Santiago que variará según la anchura de la ventana de navegación empleando la etiqueta `<picture>`y los elementos `<source>`.
			- Deberás conseguir una imagen de la catedral y obtener 2 imágenes a partir de ésta: una imagen de 800px de ancho, y otra de 480px de ancho. En este enlace puedes consultar como hacer esto con GIMP.
			- Cuando la anchura de la ventana de navegación sea >= 800px , el selector escogerá la imagen de 800px de ancho. Cando  sea <800px se mostrará la imagen de 480px de ancho. 

   - Deberá tener un pie de página con la dirección del concello.
   
Puedes usar las siguientes propiedades de estilos:
   - Para centrar el cuerpo de la página y las imágenes:  *margin: 0 auto;*
   - Para establecer la imagen de fondo de la cabecera centrada y sin repetirse::  *background: url(nomedaimaxe.jpg) no-repeat center;*
   - Para rellenar los textos y que no toquen los bordes:  *padding: 20px;*
   - Para mostrar las imágenes como elemento de bloque:  *display: block;*

Puedes usar como referencia las imágenes de la carpeta *03-imgs responsive*

## Ej4. RESPONSIVE FLEX (**2 pts**)

A partir del código HTML y CSS base, en la carpeta *04-responsive-flex*:
   - Establecer un diseño Flexbox con display: flex en el elemento contenedor main. Alinea sus items de forma que el primero se alinee al principio y el último al final.
   - Implementa una estrategia Mobile-First haciendo uso de las propiedades flex-wrap y flex-basis de manera que los elementos hijo del contenedor ocupen un 100% de la anchura del contenedor. Ref: imagen *pantalla_movil*
   - Para pantallas de tablets y equipos de sobremesa, i.e, de más de 600px, modifica las propiedades anteriores de manera que los elementos hijo no fluyan, i.e, el diseño se mantenga como columnas dentro de una sola fila con 3 columnas. Ref: imagen *pantalla_tablet*
