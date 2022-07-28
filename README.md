## ¿Qué es el Frontend?
---
En el desarrollo web, el frontend es toda el área visual que un usuario puede ver e interactuar en un sitio web. Desde componentes más pequeños como botones, entradas de texto, imágenes hasta toda página en general. Todo lo que podemos visualizar como texto, imágenes, otros posts, botones, links de redirección, página de perfil de usuarios, podcasts, forman parte del frontend del sitio.

## ¿Qué es el desarrollo Frontend?
---
Bueno como ya habrás supuesto, el desarrollo frontend se encarga de construir las vistas de un sitio web, utilizando herramientas especializadas que ayudan y facilitan su creación. Es importante destacar que, aunque este puesto se encargue de la parte visual, no le compete el diseño de la web, es decir, para la construcción de un sitio, primero se debe pasar por el proceso de diseño (que normalmente se encarga un diseñador), y luego con esto el desarrollador frontend procede a maquetar dicho diseño. Sería un buen plus que la persona que se encargue del frontend sepa diseñar, no es una tarea que se le deba delegar necesariamente, pero si lo sabe pues también es bueno.

Otra tarea importante de un desarrollador Frontend y que en ocasiones se desconoce cuando se comienza es la implementación de los servicios que el sitio web consumirá. En la mayoría de los casos nuestra web (a no ser que sea un sitio totalmente estático o sin funcionalidades) estará consumiendo servicios que provienen de otras fuentes y que normalmente realiza un desarrollador backend  como por ejemplo una API REST. Estos servicios deben ser implementados por el desarrollador frontend para su uso en la web.

Ahora bien, para poder construir una web, requiere de ciertas tecnologías que son la base.

![html](https://res.cloudinary.com/practicaldev/image/fetch/s--oR_XMEm4--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/wehzu33fvfxiq39wyu03.jpg)

- **HTML (HyperText Markup Language):** Es un lenguaje de marcado de hiper texto. Con él  construimos la estructura inicial de un sitio web. El HTML viene siendo el esqueleto de una web, que contiene el texto a mostrar. Se basa en etiquetas para poder construir todo el sitio web. Ejemplo, el siguiente código muestra un párrafo:
```html
<p> Esto es un párrafo </p>
```

![css](https://res.cloudinary.com/practicaldev/image/fetch/s--iBoT89OE--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/lpymwa9hneibpgkmc6rp.jpg)

- **CSS (Cascading Style Sheets):** Es un lenguaje de estilos en cascada, esto le proporciona a la web los colores, espacios, tamaños, tipografías que necesita para poder tener el diseño que se quiere construir. CSS se construye por medio de reglas de estilos y que influyen sobre los archivos HTML que existen. Ejemplo, el siguiente código les da un color rojo a todos los párrafos:
```css
p {
  color: red;
}
```	
![js](https://res.cloudinary.com/practicaldev/image/fetch/s--NLVCcNCN--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/l2m99wgn3opzse769aa9.png)

- **JavaScript:** Es un lenguaje de programación que en los últimos años ha tenido un gran crecimiento, es usado por una gran comunidad y cada año es mantenido y recibiendo actualizaciones que le permite mejorar. Con JavaScript podemos darle interacción a nuestro sitio web. Hasta los momentos con puro HTML y CSS podemos crear un sitio estático, pero con JavaScript le damos el dinamismo que necesitamos que tenga nuestra web. JavaScript es un lenguaje que si o si debes aprender para ser todo un profesional. Además de él se desglosan una gran cantidad de herramientas para facilitar nuestro trabajo del día a día. Ejemplo, en el siguiente código renombra el texto del párrafo:
```javascript
    document.getElementByTagName("p").innerHTML = 'Este es un nuevo párrafo'
```	
RoadMap de un desarrollador Frontend
[enlace](https://roadmap.sh/frontend)


# SPA (Single Page Application)
Una single-page application (SPA), o aplicación de página única, es una aplicación web o es un sitio web que cabe en una sola página con el propósito de dar una experiencia más fluida a los usuarios, como si fuera una aplicación de escritorio. 

En un SPA todos los códigos de HTML, JavaScript, y CSS se cargan una sola vez​ o los recursos necesarios se cargan dinámicamente cuando lo requiera la página, normalmente como respuesta a las acciones del usuario. 

La página no tiene que cargarse de nuevo en ningún punto del proceso y tampoco es necesario transferir a otra página, aunque las tecnologías modernas (como el pushState() API del HTML5) permiten la navegabilidad en páginas lógicas dentro de la aplicación. 

La interacción con las aplicaciones de página única pueden involucrar comunicaciones dinámicas con el servidor web que está detrás.

El término single-page application fue utilizado por Steve Yen en 2005, aunque el concepto ya había sido discutido en el año 2003.

Stuart Morris escribió una página web de página única slashdotslash.com que tenía las mismas metas y funciones en el año 2002

En el mismo año Lucas Birdeau, Kevin Hakman, Michael Peachey y Evan Yeh describieron las implementaciones de aplicaciones de página única en la patente estadounidense 8,136,109.

Los navegadores modernos que pueden parsear HTML5 permiten a los desarrolladores cambiar la Interfaz del usuario y las aplicaciones lógicas de los servidores hacia los clientes. 

Bibliotecas de código abierto soportan la creación de un SPA sin forzar al desarrollador entrar a lo profundo de JavaScript y pelearse con los problemas de la tecnología.

## Diferencias:
## Multi-page 
En primer lugar vamos a entender lo opuesto a un SPA, el cual vendría ser un MPA. Es decir que las navegaciones dentro de nuestra web obliga a nuestro browser a recargar todo el contenido de nuevo, es decir que los css, javascript, imágenes, html y demás contenidos volverán a ser cargados.

Nota: _usualmente los browsers meten en cache los archivos estáticos como javascript, hojas de estilos, imágenes, video para agilizar la carga de las páginas web._


## Single-page-aplication
Por otro lado, los SPA son aplicaciones web que se ejecutan en una sola página, es decir que una vez ha sido cargada la página inicial toda la navegación del proyecto será por medio de dicha página evitando de esta manera refrescar el browser.

Se suele hacer uso de un framework o librerías JavaScript para lograr el cometido, ya que estas implementan todo lo necesario para crear un proyecto SPA y para consultar el contenido al servidor como podría ser un listado de usuarios se haría a través de AJAX o WEBSOCKETS.

Analicemos la siguiente imagen:
![img](https://anexsoft.com/storage/app/media/posts/spa/SPA.jpg)

- El layout es nuestra plantilla de nuestro proyecto que abarca el header, content y footer. Por ende, el contenido principal de la web ya se cargó.

- El content será cambiado dinámicamente en función a la URL que estemos navegando. Es decir, que nuestro SPA va asociar la URL o ruta por la que estamos navegando con una página que reemplazará lo que hay en el content.

### Ventajas
- Agiliza la lógica de negocio al procesarse en lado del cliente como bien podría ser cálculos de impuestos, sumatorias, etc.

- Agiliza la navegación ya que todo el contenido inicial (css, js, imágenes, etc) es cargado de golpe, lo demás será el contenido que se quiera visualizar.

- Ayuda abaratar los costos de servidor al dismunir el número de requests realizados.

### Desventajas
- Se pierde el SEO, aunque hay formas de evitarlo no es algo natural en un SPA ya que los robots no leen o interpretan contenido cargado en segundo plano.

- La primera carga puede tardar un poco ya que el peso del proyecto estará en función al tamaño de este.

- Curva de aprendizaje, nos obliga aprender nuevos frameworks o librerías para evaluar cual será la más adecuada para nuestro proyecto. En el mercado tenemos frameworks sencillos o más complejos de aprender que en función hacen lo mismo pero agregan o quitan conceptos alargando o disminuyendo la curva de aprendizaje.

### Que tipos de proyectos es recomendable usar un SPA?
- En realidad puede ser usado para cualquier tipo de proyecto pero los más recomendados en mi experiencia personal serían:

- Aplicaciones móviles web.

- Aplicaciones Back-Office para administrar una web. Por ejemplo, el administrador de una página hecha en Wordpress podría ser un SPA.

- Aplicaciones de INTRANET.

- Aplicaciones comerciales como un e-commerce personalmente creo que debemos enfocarnos en multi-page application haciendo uso de una tecnología back-end como PHP, .NET o lo que sea.

# Web Components

Los Componentes Web son un paquete de diferentes tecnologías que te permiten crear elementos personalizados reutilizables — con su funcionalidad encapsulada apartada del resto del código — y utilizarlos en las aplicaciones web.

- **Conceptos y uso**
Como desarrolladores, sabemos que reutilizar código tanto como sea posible es una buena idea. Esto tradicionalmente no es sencillo para estructuras de marcado personalizadas — piense en el complejo HTML (y sus estilos y scripts asociados) que en ocasiones se han tenido que escribir para renderizar controles de interfaz (UI) personalizados, y ahora usarlos múltiples veces puede crear un caos en la página si no se es cuidadoso.

- **Los Componentes Web** apuntan a resolver dichos problemas — consiste en tres tecnologías principalmente, las que se pueden usar juntas para crear elementos personalizables versátiles que encapsulan la funcionalidad y pueda ser reutilizada donde sea sin miedo a colisiones de código.

- **Custom elements (elementos personalizados):** Un conjunto de APIs de JavaScript que permiten definir elementos personalizados y su comportamiento, que entonces puede ser utilizado como se deseé en la interfaz del usuario.

- **Shadow DOM:** Un conjunto de APIs de JavaScript para fijar un árbol DOM "sombra" encapsulado a un elemento — que es renderizado por separado del documento DOM principal — y controlando funcionalidad asociada. De esta forma, se pueden mantener características de un elemento en privado, así puede tener el estilo y los scripts sin miedo de colisiones con otras partes del documento.

- **HTML templates (plantillas HTML):** Los elementos template y slot permiten escribir plantillas de marcado que no son desplegadas en la página renderizada. Éstas pueden ser reutilizadas en múltiples ocasiones como base de la estructura de un elemento personalizado.

La aproximación básica para implementar un componente web, generalmente es la siguiente:

1. Crear una clase o función en la cual especificar la funcionalidad del componente web. Si se usa una clase, usar la sintaxis de ES2015 (ver Clases para más información).

2. Registrar el nuevo elemento personalizado utilizando el método CustomElementRegistry.define(), pasándole el nombre del elemento a ser definido, la clase o función en la cuál su funcionalidad esta especificada, y opcionalmente, de que elemento hereda.

3. Si se requiere, adjuntar un shadow DOM al elemento personalizado usando el método Element.attachShadow(). Añadir elementos hijos, oyentes de eventos, etc., al shadow DOM utilizando métodos normales del DOM.

4. Si se requiere, definir una plantilla HTML utilizando <template> y <slot>. Nuevamente usar métodos regulares del DOM para clonar la plantilla y acoplarla al shadow DOM.

5. Utilizar los componentes personalizados en la página web cuando se desee, como se utilizaría cualquier otro elemento HTML.
