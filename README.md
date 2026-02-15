# HTML Breakfast
Ejercicio para practicar etiquetas HTML:

## Objetivo
Estructurar el contenido de una página web mediante etiquetas HTML.

## Instrucciones

- Utiliza la lista de etiquetas que se adjunta para crear algo similar al siguiente diseño:

[Urban Toast](https://imgur.com/DhgcTot.png)

### Iteración 1

- Haz un "fork" de este proyecto y clona el contenido desde tu repositorio.

### Iteración 2: Etiquetas de `<head>`
- Dentro del fichero `index.html`, busca las etiquetas correctas para introducir el siguiente contenido:
   - Idioma de la página: inglés
   - Caracteres utf-8 (Busca cual es el significado de estas siglas)
   - Título de la página que aparece en la pestaña del navegador: Urban Toast
### Iteración 3: Etiquetas de `<body>`
- Crea una barra de navegación con los siguientes enlaces: HOME, ABOUT US, DAILY OFFER, CONTACT US
- Título principal: The good breakfast
- Párrafo 1: Here you will find all sorts of delicious treats
- Imagen: https://i.postimg.cc/htxcJGB6/ZKkCecn.jpg
- Pie de foto: powered by biscuit.
- Párrafo de pie de página: From the oven with love

### Iteración 4: Párrafos
- Inserta el siguiente texto que explica algo sobre el restaurante:
"Our commitment is to use impeccable sourcing and quality ingredients to help 
  you code.An ongoing collaboration between the classroom staff and the development
   team allow us to iterate our content and give our students the coding 'fruits and
    vegetables' -mainly made of JavaScript- that they need to grow as a healthy 
    developer."
- Resalta las palabras "quality ingredients" con la etiqueta de texto importante

### Iteración 5: Texto preformateado
- Utiliza la etiqueta de texto preformateado e introduce la siguiente frase:  "Good code & good coffee, everyday"

### Iteración 6: Listas
- Crea un menú para indicar el café que servimos.
- Introduce una cabecera que indique el menú.
- Una lista de Cafés: Café latte, American, Machiatto, Capuccino
- Una lista de tés: Earl Grey, Green Tea, Rooibos

### Iteración 6: Bonus
- Transforma la lista anterior en una tabla.

### Iteración 7: Formulario de Reservas
- Crea un formulario de reservas, con el título "Reservas Aquí", para recoger la información de una reserva:
  - Una caja con etiqueta para recoger el nombre del cliente.
  - Una selección de opciones para elegir entre Snack or Breakfast
  - Una selección de opciones para elegir cuántas personas serán (de 1 a 4).
  - Un botón para enviar la información

### Iteración 8: Elementos del pie de página
- Añade un link ‘Contact Us’ en la sección del pie de página. Debería abrir la aplicación de correo del usuario para poder enviar un mail al equipo.
- Muestra el horario de apertura del restaurante

### Validaciones:

- Comprueba que tu página está correctamente estructurada con la herramienta: https://validator.w3.org/

## Lista de Etiquetas

**Estructura Básica y Metadatos**

* **`<!DOCTYPE html>`**: Define el tipo de documento y la versión de HTML.
* **`<html>`**: Elemento raíz que encierra todo el contenido de la página.
* **`<head>`**: Contenedor de metadatos (información no visible) como título y enlaces a estilos.
* **`<body>`**: Contiene todo el contenido visible del documento (texto, imágenes, enlaces).
* **`<meta>`**: Define metadatos como la codificación de caracteres y la configuración del viewport.
* **`<title>`**: Establece el título de la página que aparece en la pestaña del navegador.
* **`<link>`**: Enlaza recursos externos, comúnmente usado para hojas de estilo CSS.

**Texto y Formato**

* **`<h1>` a `<h6>**`: Encabezados de sección, donde `<h1>` es el más importante y `<h6>` el menos.
* **`<p>`**: Define un párrafo de texto.
* **`<br>`**: Inserta un salto de línea simple.
* **`<strong>`**: Define texto con fuerte importancia (generalmente en negrita).
* **`<em>`**: Define texto enfatizado (generalmente en cursiva).

**Contenido y Medios**

* **`<a>`**: Crea un hiperenlace a otras páginas web, archivos o ubicaciones dentro de la misma página.
* **`<img>`**: Inserta una imagen en el documento. Requiere el atributo 'src' y 'alt'.
* **`<ul>`**: Define una lista desordenada (con viñetas).
* **`<ol>`**: Define una lista ordenada (con números o letras).
* **`<li>`**: Define un ítem dentro de una lista (ya sea ordenada o desordenada).

**Estructura Semántica**

* **`<div>`**: Contenedor genérico de bloque para agrupar elementos y aplicar estilos.
* **`<span>`**: Contenedor genérico en línea para aplicar estilos a partes de texto.
* **`<header>`**: Define la cabecera de una página o sección.
* **`<nav>`**: Define un conjunto de enlaces de navegación.
* **`<main>`**: Especifica el contenido principal y único del documento.
* **`<section>`**: Define una sección temática en el documento.
* **`<article>`**: Representa contenido independiente y autónomo (como un artículo de blog).
* **`<aside>`**: Contenido relacionado indirectamente con el contenido principal (barra lateral).
* **`<footer>`**: Define el pie de página de un documento o sección.

**Tablas y Formularios**

* **`<table>`**: Crea una tabla para mostrar datos tabulares.
* **`<tr>`**: Define una fila en una tabla.
* **`<th>`**: Define una celda de encabezado en una tabla.
* **`<td>`**: Define una celda de datos estándar en una tabla.
* **`<form>`**: Crea un formulario para recolectar datos del usuario.
* **`<input>`**: Campo de entrada de datos variable según su atributo 'type' (text, email, password, etc.).
* **`<label>`**: Etiqueta descriptiva para un elemento de formulario.
* **`<button>`**: Botón clicable para enviar formularios o ejecutar acciones.
