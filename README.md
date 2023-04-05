# M04-UF1: PabloLopez2.github.io
Cyber: Llenguatges de Marques (M04 - UF1)

## Página web de ejemplo de Lenguajes de Marcas (M04UF1)

Esta página es un test a modo de CV.

## Lista de tareas a hacer en la página

- [x] Crear plantilla del cuerpo HTML

- [x] Añadir navegación

- [x] Crear estilo básico

# XML, DTD, Markdown, HTML, CSS y JavaScript

## Apuntes XML (Extended Markup Language)

### XML, un poco de historia

**XML** *(Extended Markup Language)* es el lenguaje base de los lenguajes de marcas que tenemos hoy en día. XML no viene de la nada. En los años 70 era **SGML**, se utilizaba para marcar en documentos lo que era una **negrita**, una *cursiva*, ~~tachado~~ etc. Ya que en aquella época no había *interfaz gráfica*. El *driver* de la impresora **interpreta** esto, es decir, lo **parseaba** y ponía las **negritas**, *cursivas*… cuando tocaba. Llegan los 90, aparte de inventarse Linux, se inventa **Internet**. 


### ¿Qué son las marcas y qué son los documentos?

Las **marcas** son los elementos que se utilizan para *estructurar el contenido del documento*. Tienen su **apertura** y su **cierre**. Para cerrar las etiquetas se pone una **/**. Por otro lado, el documento XML es el archivo que *contiene la información estructurada utilizando marcas*. 

Las **marcas** se refiere al texto que se tiene que **parsear**, es decir *interpretar*, el programa lo interpreta. El parseador tiene que leer el texto plano y cuando lo muestra en pantalla, ha de mostrar el texto en negrita `<B>hola</B>` o en cursiva, `<I>IAN</I>` o __subrayar__ `<U>Guillem</U>` → esto de las letras que están entre picos se le llaman marcas o etiquetas. `<P>` (párrafo) `<a>` (link).

### Historia de los navegadores (o buscadores)

*Microsoft* , en los años 90, creó el primer browser, se llamaba Mosaic. Netscape creó un navegador donde tenía sus suscripciones de pago como el correo electrónico entre ellos. En su día, internet no servía de nada si no tenías un navegador. 

Microsoft vino con su **internet explorer**, habló con todos los proveedores de internet para que incluyeran su navegador y en algunos casos para no incluyeran **Netscape**. Además, Microsoft implementaba su navegador Internet explorer como **parte del núcleo y no se podía desinstalar**, *era parte del sistema operativo*. Esto fue una batalla que acabaron en juicio, ya que es un movimiento monopolístico. Pues al final internet explorer **se cargó a todos**, incluido Netscape. 

**Internet explorer** interpretaba muy mal **HTML** y no seguía un *estándar* y **Netscape** si. A los años 2000 Netscape cierra. Pero hace un último tiro, antes de que Netscape cerrase creó una fundación con los últimos dineritos que tenía para generar un proyecto que respetara todo lo posible los estándares de la web, *liberó su código* y creó **mozilla** y proyectos como **FireFox**. Durante los años 2000, hasta llegar Chrome (2008), consiguió un **más de un 30% del mercado**, y la gente empezó a hacer las páginas *bien*. 

También sobre los años 2000 se creó un **consorcio**, **W3C**. Un consorcio es una comunidad que tiene sus estatutos, sin ánimo de lucro y si te inscribes es porque tienes unas responsabilidades. Aquí definieron unos estándares de internet, rígidos a la hora de cumplirlo y flexible para ir evolucionando.

### Historia de HTML4, XML y XHTML

**HTML 4** no seguía ningún *estándar*. No se sabía cuando cerraban las etiquetas por ejemplo. Entonces, decidieron crear **XML** (Extended markup languages), donde definía estas normas *rígidas* pero *flexibles* (buen oxímoron) para poder crear lo que queramos. Xml define las normas de como hacer las etiquetas, no las etiquetas en sí, es decir todas las etiquetas que se abren se tienen que cerrar. **No impone visualización, impone estructura**.

Después salió **XHTML** de los 1998 hasta 2008, que es HTML4 pero con la capa de filtros de XML. Aquí Microsoft lo pasó un poco mal ya que todas las empresas empezaron a seguir estos estándares sufrió muchas denuncias. Intentó seguir los estándares pero no como todos pensabamos.

### Historia de Flash Player y la etiqueta vídeo.

Se ve, que antes **JavaScript** no lo tomaban en serio y decían que era un chiste. Pues algunas empresas decidieron utilizar **Flash** (privativo), bueno pues hubo **los mayores hacks de la historia**, incluso llegaron a poner **~~nopor~~** en webs de bancos que utilizaban flash. 

Llegaron los móviles y las tablets, que no iban a soportar Flash, ya que solo lo controlaba una empresa y HTML5 muchos más, (esto a lo largo de 2008), y bueno pues vino con una etiqueta nueva como *draft*, la de **vídeo**. Entonces **cada navegador implementaba el formato de vídeo que a él le interesaba más**, por ejemplo **Safari** era el *.mov*, **Internet Explorer** era *MP4*, **FireFox** tenia el *.ogv* que era el **estándar** (humilde). Hoy en día MP4 es libre, antes no, aunque es más conocido .ogv.

Por otro lado, se implementó la etiqueta **audio** como *draft* también (aunque de manera eficiente se implementó en el 2012), en 2012, los navegadores empezaron a implementar bien HTML5.

### Microsoft Edge, Chrome y Chromium

Microsoft decide crear **Microsoft Edge** en el año 2012 porque nadie utilizaba ya Internet Explorer pero era literalmente internet explorer pero un poco mejor. Se creó **Chromium** con la interfaz de **Edge**. Es **Chrome** en Linux, open source, Servia para hacer tu propio navegador. Chrome no utilizo chromium, si no KHTML. WebKit es la base de chromium, safari, Edge. Hemos de saber que HTML5 está diseñado para ir evolucionando.

Para acabar con la historia, hay una frase que me gustaría citar:
>Nadie es más odiado que aquel que dice la verdad. Platón.

## Comenzamos a crear nuestro primer archivo XML

### Archivos de texto plano, enriquecido y binario:
* **Texto plano** →  archivo que contiene texto sin formato o estructura, es decir, simplemente una secuencia de caracteres. El texto plano es legible para los humanos y se puede abrir y editar con un editor de texto simple.
    * *Formatos* → VIM, Notepad, archivos de Kotlin, Python, C++, documentos.txt, docx etc.

* **Texto enriquecido** → Es un texto plano con info extra. Se refiere a un archivo que contiene texto con formatos adicionales como negritas, cursivas, subrayados, tamaños de fuente, colores, etc. Por ejemplo, mis apuntes de Google Docs son texto enriquecido. 
    *  *Formatos* → HTML, RTF, DOC. 

* **Binario** → Contienen datos en un formato que no es legible directamente por los humanos, sino que está diseñado para ser procesado por ordenadores. 
    * *Formartos* → Imagen JPEG, PNG, archivos de audio MP3, .MP4, archivos sql.

### Tipos de etiquetas
>**cabecera →** `<?xml version="1.0" encoding="UTF-8" ?>.`
>>Esto indica a nuestro programa o a la librería que utilizamos internamente de programación, que es lo que vamos a leer, qué codificación y que versión del estándar es.

>**Para comentar →** `<!-- texto -->`

* Etiquetas pares:
	* Se abren y cierran, Cuando lo que tenemos que escribir es muy variable, puede ser par (character por ejemplo, o cuando algo vaya a contener muchos datos)

* Etiquetas impares:
	* Se cierran en sí mismas. Por ejemplo la edad, es una cosa muy concreta, entonces es recomendable hacerla impar.


### Ejemplo de atributo o propiedad
> **\<age value="197" />** → Value es un atributo o propiedad. Un atributo es una propiedad que se define dentro de la etiqueta de un elemento y proporciona información adicional sobre ese elemento. 
	
*Cosas a tener en cuenta:*

Todo archivo XML, necesita una **etiqueta raíz**, una etiqueta donde dependen el resto de elementos (como el root), lo ideal es que represente algo (ej: character) y **toda etiqueta raíz debe cerrarse**. 
Eso sí, es importante escribir en inglés, no hay que escribir ñ, ç, ´, (no poner anio, anyo, o ano).

>**UTF-8** → ignifica que incluye todos los carácteres (sistema de codificación universal) incluidos extraterrestres (emojis). 

XML sirve para construir los datos como queremos. Estamos diseñando un formato, si hacemos las etiquetas impares en age, hemos de hacerlo para todos los personajes.

Lo bueno de XML, es que podemos aportar información de cada elemento, no como en una base de datos. 

### Código en XML:
```XML
<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE character SYSTEM "character.dtd">
<character id_character="1">
	<name>Eustaquio</name>
	<surname>Mendoza</surname>
	<!-- Comentario -->
	<age value="197" />
	<race>Enano</race>
	<class>Artificiero</class>
	<gender abbrev="N">Non-Binary</gender>
	<height cm="130" />
	<weight kg="80" />
	<language abbrev="prt">Portugués</language>
	<TieneLaEso />
	<weapons>
		<weapon id_weapon="1" />
		<weapon id_weapon="3" />
		<weapon id_weapon="7" />
		<weapon id_weapon="1" />
	</weapons>
</character> 
```
---

## Apuntes DTD (Document Type Definition)

**DTD** *(Document Type Definition)*. Es un conjunto de reglas que especifican la estructura, los elementos y los atributos que puede contener un documento **XML**.

El propósito de una DTD es establecer una **estructura bien definida y coherente** para un tipo específico de documento XML, lo que ayuda a garantizar que el documento se pueda *interpretar* y _procesar_ correctamente por cualquier sistema informático que lo use.

**DTD** es más antiguo que **XSD** *(XML Schema Definition)* y **DTD** es *universal*, se interpreta bastante más fácil, los bancos lo usan. También se utiliza para *validar*.

El **orden de validación puede variar según tu gusto**: Puedes poner primero `<!ELEMENT>` que es una *declaración*, seguido de el **término técnico** que se refieren a un *tipo de contenido permitido en un elemento*, como por ejemplo **#PCDATA** y justo abajo la otra *declaración* (si es que tiene) `<!ATTLIST>` que se refiere a la declaración de los *atributos*.

Terminos técnicos:

* **#REQUIRED**: Esta etiqueta se utiliza para especificar que un atributo es obligatorio para un elemento determinado. Si un atributo con esta etiqueta no se especifica en el documento XML, se produce un error de validación.

* **#PCDATA**: Esta etiqueta se utiliza para especificar que un elemento puede contener solo datos de texto plano (texto sin formato), sin etiquetas XML ni caracteres especiales. Es decir, el elemento no puede contener sub-elementos, solo texto.

* **#EMPTY**: Esta etiqueta se utiliza para especificar que un elemento no puede contener contenido. Es decir, un elemento con esta etiqueta no puede tener texto o sub-elementos. Se utiliza para elementos que actúan como contenedores vacíos, como las etiquetas de salto de línea, las etiquetas de cierre, etc.

### Código en DTD
```DTD
<!ELEMENT character (name, surname, age, race, class, 
	height, weight, language, TieneLaEso, weapons?)>

<!ELEMENT name (#PCDATA)>
<!ELEMENT surname (#PCDATA)>
<!ELEMENT age EMPTY>
<!ELEMENT race (#PCDATA)>
<!ELEMENT class (#PCDATA)>
<!ELEMENT gender (#PCDATA)>
<!ELEMENT height EMPTY>
<!ELEMENT weight EMPTY>
<!ELEMENT language (#PCDATA)>
<!ELEMENT weapons (weapon*)>
<!ELEMENT weapon EMPTY>

<!ATTLIST character id_character CDATA #REQUIRED> 
<!ATTLIST age years CDATA #REQUIRED> 
<!ATTLIST gender abbrev CDATA #REQUIRED> 
<!ATTLIST height cm CDATA #REQUIRED> 
<!ATTLIST weight kg CDATA #REQUIRED> 
<!ATTLIST language abbrev CDATA #REQUIRED> 
```

---

## Apuntes MarkDown

MarkDown sirve para documentar, estos son los apuntes de MarkDown:

`*cursiva*` → esto en markdown se le llama enfasis

### Listas
* uno
	* sub apartado 1
* dos
	* sub apartado 2
* tres
	* sub apartado 3
	
### Citas
> Esto sirve para citar
> para destacar cosas concretas
> como un codiguito
>> Esto es una cita **dentro** de una _cita_ 


### Enlaces

Enlace
[CondorChem](https://condorchem.com)

Y [ESTO](http://enti.cat) es otro enlace

### Imagen incrustada
![Descripcion de la imagen](https://5.imimg.com/data5/SJ/GR/TW/SELLER-63202466/ventorlin-inhaler-500x500.jpg)


### Ejemplo de resaltado de sintaxis

```kotlin
fun printOnlyOdds(list: List<Int?>) {

    for (element in list) {
        if ((element?.rem(2) ?: 0) != 0) {  //rem = remainder %
            print("$element ")
        }
    }
}
```

### Listas de tareas
- [ ] Primera tarea
- [X] Segunda tarea
- [ ] Tercera tarea



### Carácteres extendidos
:poop: :alien: :cry: :imp: :relaxed: :laughing: :cherries: :rat:


### Estilo de caracteres

*cursiva* _cursiva_

**negrita** __negrita__

~~TACHADO~~

~~***tachado negrita u cursiva***~~

### Tablas
| id_character | name      | age | level |
| ---:         | ---:      | ---:| ---:  |
| 1            | Eustaquio | 197 | 99    |
| 2            | Mariana   | 20  | 100   | 
| 3            | Mortadelo | 100 | 1     |
| 4            | Messi     | 44  | 99    |


### Escapar caracteres
\# escapar 

\*escapar*

---

## APUNTES HTML (Hypertext Markup Language)

Se creo para usarse con HTTP. 
* HTTP salio en 1991.
* HTML en el 1993.

En 1991 **Tim Berners-Lee** creo **HTTP** y con ello las bases de **HTML**. Hasta ese entonces (1991) no habia herramientas para comunicarse o transferir información por **Internet**.

### WWW

Antes de saber acerca de WWW (www.google.es), tenemos que saber que es el **.es**. A esto se le llama **TLD** (Top level domain). Cuando introducimos una pagina web como la anterior en el navegador, lo primero que se lee es el **.es** .

>El **DNS** se guarda el **TLD**, de esta manera es mas rapido y mas fácil de clasificar. Todos los servidores de DNS empiezan a leer por el TLD.

Al principio solo habia 3 TLDs : 
* .com 
* .edu 
* .net

**Todos ellos pertenecian a Estados Unidos, que se los quisieron quedar para ellos aunque al final no pudieron**

Ponemos **WWW** para diferenciarlos del resto de servicios. Antes se podia acceder por el navegador a una web y utilizar FTP para transferir archivos (*ftp.ubuntu.com*). WWW remarca que cuando nos conectamos a esa direccion, con ese prefijo, nos vamos a conectar al puerto **80**.

Actualmente si por ejemplo entramos a enti.cat, el navegador utiliza HTTPS (no HTTP) y utiliza el puerto correspondiente. Hoy en dia no se le da importancia a veces a www . Lo mas habitual es: **Mantenerlo y que se vea.**, **Hacer una redireccion de salto.**

### Comenzamos HTML (HTML 5 o LIFE SCHEME)

> Life scheme hace referencia a que esta continuamente evolucionando.

Internet explorer estuvo en guerra con Netscape, y se lo cargo.
Cuando murio Netscape, fue liberado por la fundacion Mozilla. Su objetivo es hacer un navegador que respete los estandares web. Despues salion Opera, Chrome y todos sus derivados.

>Firefox no depende de ninguna compañia (es open-source).
>Opera no es muy fiable por temas de seguridad.

Hoy en dia todos respetan bastante el Life scheme.

Durante el HMTL4 y el LIFE SCHEME (5) hubo otro. XHTML, que consistia en:

* Una mezla de XML y DTD.
* Algunas mejoras de HTML4.

>Netscape habia hecho tan bien el motor, que hacer que interpretara las malas practicas de Microsoft fue imposible, y murio.

### Tipos de Etiquetas

Todos los documentos HTML empiezan con un **index.html.**
Todo texto o elemento ha de ir dentro de una etiqueta de **bloque**.

**Etiqueta de bloque** → Se utilizan para crear bloques de contenido que empiezan y terminan en una nueva línea, creando una división visual clara en el diseño de la página. `<p>ola k ase</p>` (la p es de párrafo), `<ul>Lista</ul>`
**Etiqueta en línea** → Se utilizan para elementos de contenido más pequeños y para elementos que no requieren una nueva línea.`<a>`, `<img>`, `<input>`, `<em>`, `<strong>`.

>HTML5 no solo definia un estándar, si no que también le daba significado.
>>**La semántica es lo que es y lo que significa.** 

La semántica en HTML5 es importante porque permite que el contenido de una página web sea más fácilmente **interpretado** por los navegadores, lectores de pantalla y otros dispositivos, lo que mejora la accesibilidad y la experiencia del usuario en general.

**Todo documento HTML ha de empezar con la siguiente cabezera:** `<!DOCTYPE html>`, es el DTD. Si no la introducimos, pueden haber problemas de compatibilidad y que se interprete mal.

### Etiquetas

* `<html></html>` → Etiqueta raíz
* `<head></head>` → Donde hay información de la página, o cosas que se tienen que interpretar en el body. Por ejemplo, el título de la página en la información de la pestaña.
    * `<title></title>`→ Se utiliza para definir el título de la página web que se mostrará en la pestaña del navegador.
    * `<meta></meta>` → Se utiliza para incluir metadatos de la página web, como la descripción, las palabras clave, el autor, la codificación de caracteres, entre otros.
    * `<script></script>` → Se utiliza para incluir código JavaScript que se ejecutará en la página web.
    * `<style></style>` → Se utiliza para definir hojas de estilo CSS que se aplicarán a la página web.
    * `<link />` → Enlaza archivos externos, como hojas de estilo CSS, fuentes tipográficas, íconos, entre otros.
* `<body></body>` → Abre y cierra los contenidos. Las siguientes etiquetas van dentro del body: 
* `<nav></nav>` → Representa un conjunto de enlaces de navegación que permiten al usuario moverse por diferentes secciones de un sitio web.
* `<header></header>` → Representaa la cabecera o encabezado de una página o sección. Puede contener elementos como el logotipo, el título de la página, la navegación principal, etc. Se suele ubicar al principio del body.
* `<main></main>` → Es donde irán los contenidos del body (header, nav, main y footer son siblings). Se puede tener más de un nav, pero más de un main o header no es recomendable.
* `<section></section>` → Se suele utilizar para dividir el contenido de una página en diferentes bloques.
* `<ul></ul>` → Bloque de lista, unordered list.
* `<ol></ol>` → Lista ordenada.
    * `<li></li>` → Elementos de la lista.
    * `<a></a>` → Address, es la etiqueta que transforma en hipertexto (link), tenemos que darle un hipervínculo que direccione a algo. Para ello se utilizan las propiedades o atributos → `<a href=”http://google.es”>enlace</a>`.
    * `<h1></h1>` → Cabezera número 1. Es el título de la página.
    * `<h2></h2>` → Cabezera número 2. Esta etiqueta puede contener h3, h4, h5.
    * `<p></p>` → Párrafo de texto.
    * `<img src="" />` → La etiqueta imagen cierra en sí misma, es decir, es impar. Se utiliza **src** para indicar el link de la imagen.
    * `<video></video>` → Videos.
    * `<audio></audio>` → Audios.
    * `<table></table>` → Tablas.
* `<form></form>` → Crea un formulario donde los usuarios pueden enviar información al servidor web.
    * `<button></button>` → Crea un botón. Puedes indicar si quieres que envíe el formulario o no de la siguiente manera: `<input type="button">` no envía datos, `<input type="submit">` envía datos.
    * `<label></label>` → Se utiliza paea mejorar la accesibilidad de los formularios. El atributo for se utiliza para asociar la etiqueta label con un control de formulario.
* `<footer></footer>` →  Representa el pie de página de una página o sección. Puede contener información de contacto, derechos de autor, enlaces a las redes sociales, etc. Se suele ubicar al final del body.

Etiquetas que no deberíamos utilizar:
* `<marquee></marquee>` → Mueve texto por pantalla. 
* `<blink></blink>` → El texto parpadea.

**`<head></head>`** y **`<body></body>`** se conocen como **etiquetas hermanas**, ya que están en la misma parte del árbol *(siblings)*

Pseudocódigo de HTML, para tener una idea de le estructura (aclaro que, no hace falta indentar, es solo para hacerlo más agradable a la vista):

```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>My Website</title>
    <meta name="description" content="This my website">
    <meta name="keywords" content="HTML, CSS, JavaScript, web development">
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="cybersecurity.html">Cybersecurity</a></li>
                <li><a href="games.html">Games</a></li>
                <li><a href="ethical_hacking.html">Ethical Hacking</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section>
            <h1>Welcome to my website!</h1>
            <p>Here you will find information about our services and products.</p>
            <a href="info.html" class="button">Learn more</a>
        </section>
        <section>
            <h2>Our Services</h2>
            <ul>
                <li>Virtualizators</li>
                <li>Gaming</li>
                <li>Optimization</li>
            </ul>
        </section>
        <section>
            <h2>Contact Us</h2>
            <form>
                <label for="name">Name:</label>
                <input type="text" id="name" name="name">
                <label for="email">Email:</label>
                <input type="email" id="email" name="email">
                <label for="message">Message:</label>
                <textarea id="message" name="message"></textarea>
                <button type="submit">Send</button>
            </form>
        </section>
    </main>
    <footer>
        <p>&copy; 2023 My Website. All rights reserved.</p>
    </footer>
</body>
</html>
```

Una vez hemos visto en profundidad HTML, me gustaría citar la siguiente frase:
>El verdadero error es cometer un error y no corregirlo.

---

## Apuntes CSS (Cascading Style Sheets)

Se decide "en cascada", porque todo va afectando a lo siguiente, no hace falta volver a definir las propiedades de una etiqueta de nuevo.

La etiqueta que permite cambiar el estilo de HTML es `<style></style>`. Todo elemento en bloque ha de tener:

* **MARGIN:** Margen exterior. 16px(arriba) 0(derecha) 128px(abajo) 20px(izquierda). Funciona como las agujas del reloj. El px se tiene que especificar a no ser que el valor sea 0, ya que se puede trabajar con varias unidades a parte de px.
* **PADDING:** Margen interior.

Las etiquetas que editamos dentro de la etiqueta style las llamamos **selectores**. El body a su vez tiene su propio MARGIN. Esta empujando hacia fuera.

Aunque pongamos margin 0, sobrará un pequeño espacio, y esto es porque el *body* también su propio margin, asíque si también le ponemos margin 0, se quitará el margen.

>RECORDATORIO: HTML define la estructura, CSS la forma o el estilo y JavaScript la acción.

La etiqueta `<link />` permite referenciar ciertas configuraciones como por ejemplo la configuracion de la etiqueta `<style></style>` o las hojas de estilo. Se utiliza rel para referenciar el nombre y href para introducir el nombre del archivo. Displays: Es como se muestran los elementos en bloque.

**Pseudopropiedad** →  `h1 a:hover {text-decoration:underline;}` hand over. Nos sirve para cambiar las propiedades en el momento en que el cursor pase por encima de un enlace.

**Display** → el atributo display dice como se muestran los elementos, podemos transformar elementos en línea en bloque.
Existen 3 tipos de displays: 
* Block. 
* Inline. 
* None.

Para aplicar css dentro de un archivo y que me lo pille el archivo html → `<link rel="stylesheet" href="estilo.css" />`

Código en CSS:

```CSS
html,body{
margin:0;
padding:0;
}

header{
width:200px;
padding:0 0 0 128px;
background-image:url(logo.png);
background-repeat:no-repeat;
background-size:128px;
}
#contact-main h2{
font-family:sans-serif;
text-shadow: 2px 2px #ff0000;/*x e y*/
color:#ffffff;
-webkit-text-stroke: 1px #000000
}

#contact-main form p{
display:flex;
}
#contact-main form label{
width:160px;
}

#contact-main form p:nth-child/*Pseudoselector*/(odd){
background-color:#ff0000;
}

#game-page header{
background-color:red;
}
```

## Apuntes JavaScript 

Para definir variables se utiliza la palabra let. 

JavaScript se considera un lenguaje de programación con tipado débil, lo que significa que no es necesario indicar el tipo de dato con el que estamos trabajando. A diferencia de otros lenguajes como Kotlin, no es necesario utilizar métodos como ".toString" o ".toInt" para convertir los datos a un tipo específico. En JavaScript, también es posible cambiar el tipo de dato de una variable directamente, y es posible concatenar varios tipos de datos. Si se declara una variable sin asignar un valor, su valor por defecto será "undefined".

### Console.log, variables y concatenación

```JS
console.log("ola k ase");

let variable = 33;
console.log(variable);

let palabreja = "Hola ";
let otra_palabreja = "(^_^)";
let concatenado = palabreja+otra_palabreja;
console.log(concatenado);
```
### Buclecitos

```JS
let contador =0;
while (contador < 10) {
	console.log(contador);
	contador++;
}

for (let i = 0; i<10; i++){
console.log(i);
}
```

### Condiciones

```JS
let PrimerValor = 10;
let SegundoValor = 6;

	if (PrimerValor == SegundoValor){
		console.log("Son iguales");
	}
	else if (PrimerValor > SegundoValor) {
		console.log("El valor" ,PrimerValor,"es mayor que",SegundoValor);
	}
	else {
		console.log("El SegundoValor es mayor");
	}
```

### Funciones
```JS
function saluda(nombre) {
	console.log("ola k ase", nombre)
}

saluda("JAN");
```

### Arrays

```JS
let videoconsolas = ["Nintendo Switch", "GameBoy Advance", "Nintendo 3ds", "Play Station 4"];
let malwares = ["Ransomware", "Trojan", "Worm", "BackDoor", "SpyWare", "ForkBomb"];
console.log(videoconsolas);
console.log(malwares[0][3]);
```

### Booleans
```JS
let true = true;
let false = false;

let a = 5;
let b = 10;
if (a > 0 && b > 0) {
  console.log("Son mayores que 0");
}

let edad = 15;
if (edad < 18 || edad >= 65) {
  console.log("No es mayor de edad");
}

let llueve = true;
if (!llueve) {
  console.log("Toca sortir al pati");
} else {
  console.log("Toca Smash");
}
```

En java script los parametros son opcionales.

**setInterval:** Es una funcion que ejecutará algo especifico (una funcion, por ejemplo) que le pasamos por un parámatero, en el segundo parametro indicaremos los milisegundos que se utilizaran de intérvalo. 
**clearInterval:** Con esta funcion se detiene el intérvalo.
```JS
let contador=0;

function cuenta () {
	contador++;
	document.getElementById("contador").innerHTML = contador;
}
setInterval(cuenta,1000);
```

**Importante:** No se puede poner el mismo nombre a un id y a una función.

### Objetos, Eventos y Propiedades

JavaScript es un lenguaje orientado a objetos y eventos. Programamos cosas que esperan a que sucedan cosas o eventos.
>Un objeto es algo que encapsula datos.

El objeto *document* representa el documento HTML que se está visualizando en el navegador web. Se puede acceder a este objeto desde cualquier parte del código JavaScript dentro de la página web. La función *getElementById* es un método que forma parte del objeto *document* y que se utiliza para seleccionar un elemento del HTML según su **atributo id.**

El **Árbol DOM** *(Document Object Model)* es una representación jerárquica de todos los elementos HTML de una página web que se carga en el navegador. Cada elemento HTML es un objeto en el árbol DOM y se puede acceder y manipular utilizando JavaScript.

Por otro lado, el **innerHTML** es una *propiedad* de los elementos **DOM** en JavaScript que permite obtener o establecer el contenido HTML de un elemento. 

Cuando se usa *document.getElementById()*, se busca en todo el **árbol DOM** del *documento* el *elemento* con el *atributo id* que se especifica como *argumento* en el *método*, y se devuelve un *objeto* que representa a ese *elemento* en particular.

Un **evento** es una acción que ocurre en una página web, como por ejemplo hacer clic en un botón, mover el ratón, pulsar una tecla. Los eventos son una forma de interactuar con el usuario y de hacer que la página web responda a sus acciones. La etiqueta con sus dos atributos`<input type="button" value="CLICA AQUÍ" onClick="alerta_maxima();"/>` tiene un evento que es el onClick. Recordamos que `type="button"` no envía el formulario `type="submit si"`.

### Wordpress, dominios .com y ole.es

Wordpress es un sitio donde nos permite tener un sistema de gestión de contenidos (CMS)
En los años 2000 se invirtió mucho en dominios .com, estaba ole.es que desapareció a los 2 años, y se invirtió mucha pasta y **_s'en van anar tot en orris_**, sobretodo invirtieron empresas en telefónica, también estaba Terra, y Yahoo que aún sigue vivo pero que le queda poco. Además también estaba geocities.com. Github tiene github pages, que es lo que vamos a utilizar.

### Certificados y empresas relacionadas con ello

Hemos de saber que HTTP (Hypertext Transfer Protocol) es html o lenguajes de marcas.
HTTPS s de secure, cifrado con ssl, para cifrar se necesitan certificados (certs) son códigos que permiten asegurar que esa información va a ir cifrada, los certificados no solo son para cifrar, si no que ese cifrado es válido porque ha sido validado. 

Podemos crear nosotros mismos los certificados, así que por ello se necesita **validar**, hay empresas que se encargan de esto y hay que pagar. Pero los certificados dan pasta, si no está validado el certificado el navegador salta, es decir sale la alerta de que no es un sitio seguro. Esta es la empresa más grande de certificados: https://www.verisign.com/  *(pagas 99$ al año)*. También https://letsencrypt.org/ si no queremos pagar pero tiene validez de 60 días.

Españita fue el país que dijo que los protocolos web tenían que ser cifrados. Durante los años 2000 y 2010, Verisign intentó meter miedo porque eran los más grandes a la hora de verificar certificados, entonces algunos se empezaron a dar cuenta de que daba igual quien validara el certificado mientras fuera **válido**. 
>Si se hubiesen **cifrado** las webs antes, sobre los 90 o así, se habría muerto internet porque antes había poca potencia para abrir los navegadores.

### Usuario webeditor

Para crear el usuario:
```Bash
useradd -M -d /var/www/ -s /bin/bash webeditor
passwd webeditor
chown -R webeditor:webeditor www
usermod -d /var/www webeditor
```
Podemos ver en el código que en /var/www/ no es lo mismo que /var/www , nosotros queríamos ponerlo en el directorio /www, entonces no lleba la / al final, por eso cambiamos en el último comando con el parámetro -d, y el parámetro -M es para evitar la creación del directorio de inicio del usuario.

Hemos de generar una llave ssh para el usuario webeditor:
```Bash
ssh-keygen -t ed25519 -C "your@example.com"
```

>**Consejitos:** No hay que meterse en root con byobu, cuando buscamos en man, podemos buscar con **/algo** y pasar a la siguiente iteración con la **n**, para ir hacia atrás **mayus n**, para indentar o tabular hacia atrás **mayus tab**

Para clonar nuestro directorio de github:
```Bash
git clone git@github.com:PabloLopez2/PabloLopez2.github.io.git
```

`<meta charset="UTF-8" /> `→ Esto sirve para tener los carácteres en **UTF-8**.

Ahora mismo tenemos el servidor de desarrollo (maquina) por un lado y el público (web) en otro.
En VIM → Ctrl w + - para hacer más pequeño o mas grande el script en vim o :resize 16. En modo visual s/jugador/valor reemplaza la string jugador por valor. En JavaScript, innerhtml es lo que hay dentro de la etiqueta `<p>hola</p>`

**NaN** → Not a Number

En CSS, *class* nos permite definir varias cosas que están definidas a un mismo tipo.

`<div></div>` La etiqueta div también se utiliza para aplicar estilos específicos a secciones del contenido, lo que permite un mayor control de la apariencia visual de la página.

`<span></span>` → La etiqueta span se utiliza para aplicar estilos o características específicas a partes del contenido dentro de un elemento div o cualquier otro elemento en HTML. Por ejemplo, se puede utilizar la etiqueta span para resaltar una palabra específica en una oración o para cambiar el color del texto en un párrafo.

\# → nos permite definir las propiedades de los elementos de id.

*Class* e *id* se pueden poner con - (guión) porque son variables, pero name y otros no, las variables con _ (guión bajo).
`-webkit-text-stroke` → El guión significa que aún no es oficial.
El formulario si lo envias se guarda en la **URL** *(Uniform Resource Locator).*

**Hardcodeado** → Es ser bruto. Cuando algo está "hardcodeado", significa que los valores o parámetros que se utilizan en una función o proceso están codificados directamente en el código fuente en lugar de ser definidos como variables o configuraciones externas que se pueden modificar fácilmente. 

**Mnemotécnica** → Son las cosas en las que nos basamos para asociar alguna formula o algo 
No se puede poner un id = funcion (el mismo nombre).

## Apuntes JSON

**JSON** *(JavaScript Object Notation)* es un formato de intercambio de datos *ligero* y *fácil de leer* utilizado para representar *objetos* y *estructuras* de datos en la programación. Es un formato de texto que se utiliza para *transmitir* datos *estructurados* entre diferentes sistemas, incluyendo aplicaciones web y móviles.

En un banco por ejemplo se usa XML antes que JSON, en JSON no son tan importantes los validadores, se utiliza para cosas instantáneas, pero un banco necesita validarlo todo, JSON ocupa poco y se envía rápido, es puro JavaScript y esto hace que el navegador interprete al instante el archivo, es mucho más rápido que XML y pesa menos. En amazon se usa JSON, pero si falla algo, es más seguro validar con XML.

Con JSON abrimos y cerramos con llaves. Ejemplo de código:

```JSON
{
	"id_character":2,
	"name":"Mariana",
	"age":"20",
	"race":"Hada",
	"gender":"F",
	"height":25,
	"weight":3.4,
}
```

>**Consejo de CSS:** Para cambiar solo una estructura en concreto en HTML (por ejemplo el body), podemos asignarle un id, ej: game-page y llamarlo así pero con el # en el CSS, es decir así: `#game-page`.

### Fetch, funciones asíncronas, Encapsulaciones y Promesas.

Con JavaScript podemos descargar archivos desde el servidor de manera asíncrona. Fetch es asíncrono, esto significa que puede ocurrir en el momento de la carga de la página, principalmente lo que hace es conectarse al servidor para descargarse un archivo JSON, es como un proceso que se ejecuta de manera paralela cuando cargamos la página. Se queda en segundo plano. 

Función anónima → es una función que no tiene nombre.

>**Una función asíncrona en JavaScript no devuelve un valor**. 
>>Los JSON han de ser procesados.

Las funciones asíncronas se escriben async function , todo el contenido de esta función se retorna encapsulada y se llama promesa, es un objeto especial y JS internamente puede procesar si ha habido algún error. Las funciones asíncronas siempre retornan algo, y por ello siempre tiene then (todas las funciones asíncronas han de contener un then), la cual tiene una función con 1 parámetro. si ha ido mal podemos utilizar otra cosa pero que no se suele hacer. 

>Toda función asíncrona retorna una promesa (objeto especial), y dentro de esa promesa están los datos.
>>Objeto es algo que encapsula datos.

**CORS** → son un conjunto de normas que nos permiten conectarnos a un sitio de manera remota

**Curl** → es un comando que nos permite conectarnos a sitios remotos. 





