# M04-UF1: PabloLopez2.github.io
Cyber: Llenguatges de Marques (M04 - UF1)

## Página web de ejemplo de Lenguajes de Marcas (M04UF1)

Esta página es un test a modo de CV.

## Lista de tareas a hacer en la página

- [x] Crear plantilla del cuerpo HTML

- [x] Añadir navegación

- [x] Crear estilo básico

# XML, DTD, Markdown, HTML, CSS y JavasScript

## Apuntes XML (Extendes Markup Language)

### XML, un poco de história

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
>**cabecera →** \<?xml version="1.0" encoding="UTF-8" ?>. 
>>Esto indica a nuestro programa o a la librería que utilizamos internamente de programación, que es lo que vamos a leer, qué codificación y que versión del estándar es.

>**Para comentar →** \<!-- texto -->

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

El **orden de validación puede variar según tu gusto**: Puedes poner primero **<!ELEMENT>** que es una *declaración*, seguido de el **término técnico** que se refieren a un *tipo de contenido permitido en un elemento*, como por ejemplo **#PCDATA** y justo abajo la otra *declaración* (si es que tiene) **<!ATTLIST>** que se refiere a la declaración de los *atributos*.

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
| id_character | name | age | level |
| ---: | ---: | ---: | ---: |
| 1 | Eustaquio | 197 | 99 |
| 2 | Mariana | 20 | 100 | 
| 3 | Mortadelo | 100 | 1 |
| 4 | Messi | 44 | 99 |


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

Actualmente si por ejemplo entramos a enti.cat, el navegador utiliza HTTPS (no HTTP) y utiliza el puerto correspondiente. Hoy en dia no se le da importancia a veces a WWW. Lo mas habitual es: **Mantenerlo y que se vea.**, **Hacer una redireccion de salto.**

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

### Etiquetas

