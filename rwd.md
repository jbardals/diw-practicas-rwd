% Responsive Web Design
% Adolfo Sanz De Diego
% Septiembre 2016



# El autor



## Adolfo Sanz De Diego

- EmpecÃ© **desarrollando aplicaciones web**, hasta que di el salto a la docencia.

- Actualmente soy **Asesor TÃ©cnico Docente** en el servicio TIC de la D.G de Infraestructuras y Servicios de la ConsejerÃ­a de EducaciÃ³n, Juventud y Deporte de la Comunidad de Madrid.

- AdemÃ¡s colaboro como **formador especializado en tecnologÃ­as de desarrollo**.


## Algunos proyectos

- **Hackathon Lovers** <http://hackathonlovers.com>: un grupo creado para emprendedores y desarrolladores amantes de los hackathones.

- **Password Manager Generator** <http://pasmangen.github.io>: un gestor de contraseÃ±as online.

- **MarkdownSlides** <https://github.com/asanzdiego/markdownslides>: un script para crear slides a partir de ficheros MD.


## Â¿Donde encontrarme?

- Mi nick: **asanzdiego**

    - AboutMe:  <http://about.me/asanzdiego>
    - GitHub:   <http://github.com/asanzdiego>
    - Twitter:  <http://twitter.com/asanzdiego>
    - Blog:     <http://asanzdiego.blogspot.com.es>
    - LinkedIn: <http://www.linkedin.com/in/asanzdiego>
    - Google+:  <http://plus.google.com/+AdolfoSanzDeDiego>



# IntroducciÃ³n



## Esto no es la web

![Esto no es la web. Fuente: bradfostweb.com](../img/brad_frost_1.png)

## Esto es la web

![Esto es la web. Fuente: bradfostweb.com](../img/brad_frost_2.png)

## Â¿SerÃ¡ esto la web?

![Â¿SerÃ¡ esto la web?. Fuente: bradfostweb.com](../img/brad_frost_3.png)

## EstadÃ­sticas

![EstadÃ­sticas. Fuente: gs.statcounter.com](../img/StatCounter-resolution-ww-monthly-200903-201408.jpeg)

## El desarrollador

![El desarrollador atual. Fuente: globalmoxie.com](../img/globalmoxie.png)

## Responsive Web Design

![Responsive Web Design. Fuente: flickr.com/photos/zergev/](../img/rwd.png)

## Content is like water

![Content is like water. Fuente: fr.wikipedia.org/wiki/Site_web_adaptatif](../img/content-is-like-water-bis.jpg)

## Graceful degradation

- Se **desarrolla para los Ãºltimos navegadores**, con la posibilidad de que funcione en navegadores antiguos.

![Graceful degradation.  Fuente: bradfostweb.com](../img/responsive-design-graceful-degradation.png)

## Progessive enhancement

- Se **desarrolla una versiÃ³n bÃ¡sica** completamente operativa, con la posibilidad de ir aÃ±adiendo mejoras para los Ãºltimos navegadores.

![Progressive enhancement. Fuente: bradfostweb.com](../img/responsive-design-progressive-enhancement.png)

## Beneficios (I)

- **ReducciÃ³n de costos**. Pues no hay que hacer varias versiones de una misma pÃ¡gina.

- **Eficiencia en la actualizaciÃ³n**. El sitio solo se debe actualizar una vez y se ve reflejada en todas las plataformas.

- **Mejora la usabilidad**. El usuario va a tener experiencias de usuario parecidas independientemente del dispositivo que estÃ© usando en cada momento

## Beneficios (II)

- **Mejora el SEO**. SegÃºn las Guidelines de Google el tener una web que se vea correctamente en mÃ³viles es un factor que tienen en cuenta a la hora de elaborar los rankings.

- **Impacto en el visitante**. Esta tecnologÃ­a por ser nueva genera impacto en las personas que la vean en acciÃ³n, lo que permitirÃ¡ asociar a la marca con creatividad e innovaciÃ³n.



# Ejemplos


## Matt Kersley

- <http://mattkersley.com/responsive>

![PÃ¡gina de testeo de Matt Kersley](../img/pagina-de-testeo-de-matt-kersley.png)

## dConstruct 2011

- <http://2011.dconstruct.org>

![Ejemplo RWD: dConstruct 2011. Fuente:ecbloguer.com](../img/dConstruct-2011-ejemplo-de-Responsive-Web-Design.jpg)

## Boston Globe

- <http://www.bostonglobe.com>

![Ejemplo RWD: Boston Globe. Fuente:ecbloguer.com](../img/Boston-Globe-ejemplo-de-Responsive-Web-Design.jpg)

## Food Sense

- <http://foodsense.is>

![Ejemplo RWD: Food Sense. Fuente:ecbloguer.com](../img/Food-Sense-ejemplo-de-Responsive-Web-Design.jpg)

## Deren Keskin

- <http://www.deren.me>

![Ejemplo RWD: Deren Keskin. Fuente:ecbloguer.com](../img/Deren-Keskin-ejemplo-de-Responsive-Web-Design.jpg)



# DiseÃ±o fluido



## De PX a EM

- Formula: **target Ã· context = result**

    - target - font-size que tenemos en pÃ­xeles
    - context - font-size base (por defecto 16px en la mayorÃ­a de los navegadores)
    - result - resultado que obtenemos en em

- Es recomendable indicar el cÃ¡lculo realizado junto a la regla de CSS.

## On Line

- <http://pxtoem.com>

![px to em](../img/pxtoem.png)

## Ejemplo

- Ejemplo para poner 13px por defecto y luego 18px para h1 en em:

~~~
body {
  font: 13px;
}

h1 {
  font-size: 1.3846 em;
  /* 18px/13px = 1.3846em */
}
~~~

## EM se hereda

- Importante: **las medidas em se heredan**, es decir, un elemento dentro de un elemento tomarÃ¡ como referencia el superior para calcular cuÃ¡nto es un em.

- Por ejemplo, si tenemos una caja donde hemos definido una fuente como 0.5em y dentro de esa caja otra con una fuente 0.25em, esta Ãºltima fuente tendrÃ¡ 1/4 de tamaÃ±o respecto a la 1/2 de tamaÃ±o de la fuente general.

## De PX a %

![CÃ¡lculo porcentajes. Fuente:aloud.es](../img/porcentajes.jpg)



# Sistema de rejilla


## Ejemplo

- 1 columna para xs (\<768px)
- 2 columnas para sm (â‰¥768px)
- 3 columnas para md (â‰¥992px)
- 4 columnas para lg (â‰¥1200px)

## Uso de clases

- Uso de clases en el HTML como **Bootstrap**
    - <http://getbootstrap.com/css>

## Ejemplo Bootstrap

~~~
<div class="row">
  <div class="col-xs-12 col-sm-6 col-md-4 col-lg-3">1</div>
  <div class="col-xs-12 col-sm-6 col-md-4 col-lg-3">2</div>
  <div class="col-xs-12 col-sm-6 col-md-4 col-lg-3">3</div>
  <div class="col-xs-12 col-sm-6 col-md-4 col-lg-3">4</div>
</div>
~~~

## SemÃ¡ntico

- **The Semantic Grid System**: Mediante layouts, y sin necesidad de usar clases en HTML.
    - <http://semantic.gs>

## Ejemplo semantic.gs (HTML)

~~~
<header>...</header>
<article>...</article>
<aside>...</aside>
~~~

## Ejemplo semantic.gs (CSS)

~~~
@column-width: 60;
@gutter-width: 20;
@columns: 12;

header { .column(12); }
article { .column(9); }
aside { .column(3); }

@media (max-device-width: 960px) {
  article { .column(12); }
  aside { .column(12); }
}
~~~



# ImÃ¡genes fluidas



## TamaÃ±o mÃ¡ximo

- Fijar un **tamaÃ±o mÃ¡ximo** (si la imagen no llega, se queda con su tamaÃ±o):

~~~
img {
  max-width:400px;
}
~~~

## Ancho del contenedor (I)

- Ocupar el **ancho del contenedor** (si la imagen no llega, se deforma):

~~~
img {
  width:100%;
}
~~~

## Ancho del contenedor (II)

- Ocupar el **ancho del contenedor** (si la imagen no llega, se queda con su tamaÃ±o):

~~~
img {
  max-width:100%;
}
~~~

## Ancho del contenedor (III)

- Ocupar el **ancho del contenedor hasta un mÃ¡ximo** (si la imagen no llega, se deforma):

~~~
img {
  width:100%;
  max-width:400px;
}
~~~

## Backgrounds

- Para los background usar **cover**

~~~
.background-fluid {
  width: 100%;
  background-image:
    url(img/water.jpg);
  background-size: cover;
}
~~~



# Viewport



## OrÃ­genes

- La etiqueta meta para el viewport fue **introducida por Apple** en Safari para mÃ³viles en el aÃ±o 2007, para ayudar a los desarrolladores a mejorar la presentaciÃ³n de sus aplicaciones web en un iPhone.

- Hoy en dÃ­a ha sido **ampliamente adoptada por el resto de navegadores mÃ³viles**, convirtiÃ©ndose en un estÃ¡ndar de facto.

## Â¿QuÃ© nos permite?

- La etiqueta viewport nos permite definir el **ancho, alto y escala del Ã¡rea** usada por el navegador para mostrar contenido.

## TamaÃ±o

- Al fijar el ancho (width) o alto (height) del viewport, **podemos usar un nÃºmero fijo de pixeles** (ej: 320px, 480px, etc) **o usar dos constantes, device-width y device-height** respectivamente.

- Se considera una **buena prÃ¡ctica configurar el viewport con device-width y device-height**, en lugar de utilizar un ancho o alto fijo.

## Escala

- La propiedad **initial-scale** controla el nivel de zoom inicial al cargarse la pÃ¡gina.

- Las propiedades **maximum-scale, minimum-scale** controlan el nivel mÃ¡ximo y mÃ­nimo de zoom que se le va a permitir usar al usuario.

- La propiedad **user-scalable [yes|no]** controlan si el usuario puede o no hacer zoom sobre la pÃ¡gina.

## Accesibilidad

- Es una **buena prÃ¡ctica de accesibilidad no bloquear las opciones de zoom** al usuario.

## Ejemplo

- Un ejemplo adaptable y accesible serÃ­a:

~~~
<meta name="viewport"
  content="width=device-width,
    initial-scale=1,
    user-scalable=yes">
~~~



# Media Queries



## Â¿QuÃ© son?

Un Media Query **no sÃ³lo nos permite seleccionar el tipo de medio** (all, braille, print, proyection, screen, tty, tv, etc.), **sino ademÃ¡s consultar otras caracterÃ­sticas** sobre el dispositivo que esta mostrando la pÃ¡gina.

## Ejemplo

- **Ejemplo**: aplicar distintas reglas CSS cuando el Ã¡rea de visualizaciÃ³n sea mayor que 480px.

## Distintos CSS

- SoluciÃ³n 1: **cargar distintas CSS**:

~~~
<link rel="stylesheet"
  type="text/css"
  media="all and (min-width: 480px)"
  href="tablet.css" />

<!-- tablet.css es un CSS con reglas para cuando el Ã¡rea de visualizaciÃ³n sea mayor que 480px -->
~~~

## Mismo CSS

- SoluciÃ³n 2: **definir distintas propiedades dentro del mismo CSS**:

~~~
@media all and (min-width: 480px) {

  /* aquÃ­ poner las reglas CSS
  para cuando el Ã¡rea de visualizaciÃ³n
  sea mayor que 480px*/
}
~~~

## Importar CSS

- SoluciÃ³n 3: **importar distintas hojas de estilo dentro del mismo CSS**:

~~~
@import url("tablet.css")
  all and (min-width: 480px);

  /* tablet.css es un CSS con reglas
  para cuando el Ã¡rea de visualizaciÃ³n
  sea mayor que 480px */
}
~~~

## Operador and

- Es usado para combinar mÃºltiples media features en un sÃ³lo Media Query, **requiriendo que cada funciÃ³n devuelve true** para que el Query tambiÃ©n lo sea.

## Ejemplo and

~~~
@media tv
  and (min-width: 700px)
  and (orientation: landscape) {

  /* reglas que queremos que
  se apliquen para televisiones
  con Ã¡reas de visualizaciÃ³n
  mayores de 700px siempre que
  la pantalla estÃ© en
  modo landscape */
}
~~~

## Operador 'or'

- Se pueden combinar mÃºltiples Media Queries **separados por comas** en una lista, de tal forma que si alguna de las Media Queries devuelve true, todo la sentencia devolverÃ¡ true.

- Esto es **equivalente a un operador or**.

- Cada Media Query separado por comas en la lista se trata individualmente.

## Ejemplo 'or'

~~~
@media tv,
  (min-width: 700px),
  (orientation: landscape) {

  /* reglas que queremos que
  se apliquen para televisiones,
  o para dispositivos con Ã¡reas
  de visualizaciÃ³n mayores
  de 700px, o cuando la pantalla
  estÃ¡ en modo landscape */
}
~~~

## Operador not

- Se utiliza para **negar un Media Query completo**.

- No se puede negar una caracterÃ­stica individualmente, si no solamente el Media Query completo.

## Ejemplo not (I)

~~~
@media not tv and max-width(800px),
  not screen and max-width(400px) {

  /* reglas que queremos que
  se apliquen para dispositivos
  que no sean ni televisiones
  con Ã¡reas de visualizaciÃ³n
  menores de 800px, ni pantallas
  con Ã¡reas de visualizaciÃ³n
  menores de 400px */
}
~~~

## Ejemplo not (II)

- El anterior ejemplo serÃ­a equivalente a:

~~~
@media not (tv and max-width(800px)),
  not (screen and max-width(400px)) {

  ...
}
~~~

## CaracterÃ­sticas (I)

- CaracterÃ­sticas que hacen referencia al **Ã¡rea de visualizaciÃ³n**:

    - **width**
    - **height**
    - **aspect-ratio** [4/3 | 16/9 | ...]
    - **orientation** [portrait | landscape]

## CaracterÃ­sticas (II)

- CaracterÃ­sticas que hacen referencia a la **pantalla del dispositivo**:

    - **device-width**
    - **device-height**
    - **device-aspect-ratio** [4/3 | 16/9 | ...]

## CaracterÃ­sticas (III)

- **Otras** caracterÃ­sticas:

    - **color**: El nÃºmero de bits de profundidad de color
    - **monocrome**: El nÃºmero de bits de profundidad de color, en dispotivos monocromÃ¡ticos
    - **resolution**: Densidad de pixels en el dispositivo, medido en dpi

## Min- y Max-

- A casi todas las caracterÃ­sticas se les puede adjuntar los **prefijos min- y max-**

- De hecho lo habitual es usar dichos prefijos.



# MetodologÃ­as



## Desktop VS Mobile

![Desktop first VS Mobile first. Fuente: brettjankord.com](../img/desktop-first-vs-mobile-first.png)

## Desktop First

- Consiste en **desarrollar para pantallas grandes** y posteriormente adaptar el diseÃ±o a pantallas pequeÃ±as.

## DF: utiliza max-width

- Normalmente los Media Queries utilizan **max-width**, simplificando y ajustando para las pantallas mÃ¡s pequeÃ±as.

~~~
@media all and (max-width: 320px) {
   /* Estilos para anchos
   menores a 320px */
}
@media all and (max-width: 768px) {
  /* Estilos para anchos
  menores a 768px */
}
~~~

## DF: problemas

- Los Media Query **no estÃ¡n soportados por todos los mÃ³viles**.

- La **versiÃ³n mÃ³vil termina siendo una versiÃ³n descafeinada** de la web original.

## Mobile first

- Consiste en **desarrollar para pantallas pequeÃ±as** y posteriormente adaptar el diseÃ±o a pantallas grandes.

## MF: utiliza min-width

- Ahora los Media Queries utilizan **min-width**, para ajustar el diseÃ±o a medida que aumenta el tamaÃ±o de pantalla.

~~~
@media all and (min-width: 320px) {
  /* Estilos para anchos
  superiores a 320px */
}
@media all and (min-width: 768px) {
  /* Estilos para anchos
  superiores a 768px */
}
~~~

## MF: ventajas

- Funciona en **mÃ³viles y/o navegadores antiguos** que no soportan los Media Queries.

- Normalmente la **hoja de estilos resultante suele ser mÃ¡s sencilla** que usando la otra vÃ­a.

- Empezar por el mÃ³vil nos servirÃ¡ para **determinar de una manera mÃ¡s clara cual es el contenido realmente importante** de nuestra web.

## Puntos de rotura (I)

- Normalmente:
    - 320px para el mÃ³vil,
    - 768px para el tablet,
    - 1024px para el portatil,
    - 1200px para el sobremesa.

## Puntos de rotura (II)

- Lo mejor serÃ­a que los puntos de rotura que aplicamos en los Media Query, fueran **en funciÃ³n de nuestro contenido**, en vez de en funciÃ³n del tamaÃ±o del dispositivo mÃ¡s vendido.

- La manera de hacerlo: **ir cambiando poco a poco el ancho del navegador y donde la web se rompa**, aplicar un Media Query.



# Acerca de



## Licencia

- Estas **transparencias** estÃ¡n hechas con:
    - MarkdownSlides: <https://github.com/asanzdiego/markdownslides>

- Estas **transparencias** estÃ¡n bajo una licencia Creative Commons Reconocimiento-CompartirIgual 3.0:
    - <http://creativecommons.org/licenses/by-sa/3.0/es>

## Fuentes

- Transparencias:
    - <https://github.com/asanzdiego/curso-interfaces-web-2016/tree/master/03-rwd/slides>

- Ejercicios:
    - <https://github.com/asanzdiego/curso-interfaces-web-2016/tree/master/03-rwd/src>

## BibliografÃ­a (I)

- Responsive Web Design
    - <http://www.arkaitzgarro.com/responsive-web-design/index.html>

- IntroducciÃ³n al DiseÃ±o Web Adaptable o Responsive Web Design
    - <http://www.emenia.es/diseno-web-adaptable-o-responsive-web-design>

- Tutorial: Responsive Web Design
    - <http://www.mmfilesi.com/blog/tutorial-responsive-web-design-i>

## BibliografÃ­a (II)

- Tutorial: Transforma tu web en Responsive Design
    - <http://blog.ikhuerta.com/transforma-tu-web-en-responsive-design>

- Curso responsive web design - Redradix School
    - <http://www.slideshare.net/Redradix/curso-responsive-web-design-redradix-school>

- Todo lo que necesita saber sobre Responsive Web Design
    - <http://www.ecbloguer.com/marketingdigital/?p=2635>

## BibliografÃ­a (III)

- DiseÃ±o web fluido y plantilla fluida con HTML5 y CSS3
    - <http://www.aloud.es/diseno-web-fluido-y-plantilla-fluida>

- Beneficios del Responsive Web Design en SEO
    - <http://madridnyc.com/blog/2013/01/29/beneficios-del-responsive-web-design-en-seo>

- Responsive Web Design Testing Tool
    - <http://mattkersley.com/responsive>

## BibliografÃ­a (IV)

- Responsive Web Design
    - <http://www.ricardocastillo.com/rwd.pdf>

- Responsive Design y accesibilidad. Buenas y malas prÃ¡cticas. Errores comunes.
    - <http://olgacarreras.blogspot.com.es/2014/01/responsive-design-y-accesibilidad.html>

- DiseÃ±o web adaptativo: mejores prÃ¡cticas
    - <http://www.emenia.es/diseno-web-adaptativo-mejores-practicas>

## BibliografÃ­a (V)

- TraducciÃ³n de "Responsive Web Design" de "A List Apart"
    - <http://diseÃ±owebresponsivo.com.ar>

- Responsive Design Exercise
    - <http://blog.garciaechegaray.com/2013/11/29/responsive-design-exercise.html>

## BibliografÃ­a (VI)

- EstadÃ­sticas de StatCounter
    - <http://gs.statcounter.com>

- PÃ¡gina de testeo de Matt Kersley
    - <http://mattkersley.com/responsive>

## BibliografÃ­a (V)

- Los 5 patrones del Responsive Design con FlexBox
    - <https://carlosazaustre.es/blog/los-5-patrones-del-responsive-design/>

- El futuro del CSS Grid Layout
    - <https://carlosazaustre.es/blog/css-grid-layout-css/>

- El gran poder de CSS3: FlexBox
    - <https://filisantillan.com/el-gran-poder-de-css3-flexbox/>