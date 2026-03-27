# Corrección del Ejercicio: HTML Breakfast

## Calificación: 65/100

## Resumen General

Has realizado un buen trabajo inicial con la estructura HTML y has demostrado iniciativa al agregar CSS a tu proyecto. Tu página tiene una base sólida, pero faltan varios elementos solicitados en las instrucciones. Vamos a revisar cada aspecto para que puedas mejorar.

## Análisis por Iteraciones

### Iteración 2: Etiquetas de `<head>` - COMPLETADA ✓

Has implementado correctamente:

- El idioma de la página (`lang="en"`)
- La codificación UTF-8 (`charset="UTF-8"`)
- El título "Urban Toast"

**Nota:** UTF-8 significa "Unicode Transformation Format - 8 bits". Es un sistema de codificación de caracteres que permite representar cualquier carácter Unicode, incluyendo letras de diferentes alfabetos, emojis y símbolos especiales. Es el estándar actual en la web.

### Iteración 3: Etiquetas de `<body>` - INCOMPLETA (3/5 puntos)

**Lo que has hecho bien:**

- Has creado una barra de navegación
- Has incluido el título principal "The good breakfast"
- Has añadido el párrafo solicitado
- Has usado correctamente `<figure>` y `<figcaption>` para la imagen

**Lo que falta o necesita corrección:**

1. **Navegación incompleta:** Te falta el enlace "HOME" y "DAILY OFFER" en tu barra de navegación. Las instrucciones pedían: HOME, ABOUT US, DAILY OFFER, CONTACT US. Solo tienes About Us, Menu y Contact Us.

2. **Estructura de navegación:** Has usado directamente `<ul>` dentro de `<nav>`, pero sería mejor envolver la lista dentro del `<nav>`:

   ```html
   <nav>
     <ul class="navegacion">
       <li><a href="index.html">Home</a></li>
       <!-- resto de enlaces -->
     </ul>
   </nav>
   ```

3. **Pie de foto:** Has escrito "Powered by biscuits" pero las instrucciones dicen "powered by biscuit" (singular).

4. **Pie de página:** Has añadido el párrafo "From the oven with love" correctamente.

### Iteración 4: Párrafos - PARCIALMENTE COMPLETADA (2/4 puntos)

En tu archivo [Aboutus.html](Aboutus.html):

**Problema principal:** Has usado `<span>` para resaltar "quality ingredients", pero las instrucciones pedían usar **la etiqueta de texto importante**. En HTML, esto significa usar `<strong>` o `<b>`.

**Diferencia importante:**

- `<strong>` indica que el texto es importante (significado semántico)
- `<span>` es un contenedor genérico sin significado semántico
- Para este caso, deberías usar: `<strong>quality ingredients</strong>`

**Otro detalle:** Falta un espacio después del punto en "...you code.An ongoing..." debería ser "...you code. An ongoing..."

### Iteración 5: Citas - NECESITA CORRECCIÓN (1/3 puntos)

Has usado la etiqueta `<cite>`, pero las instrucciones pedían una **cita en bloque**. En HTML, esto se hace con `<blockquote>`:

```html
<blockquote>Good code & good coffee, everyday</blockquote>
```

**Diferencia importante:**

- `<blockquote>` es para citas extensas que ocupan un bloque separado
- `<cite>` se usa para referenciar el título de una obra o la fuente de una cita
- `<q>` se usa para citas cortas en línea

### Iteración 6: Listas - PARCIALMENTE COMPLETADA (2/5 puntos)

En tu archivo [menu.html](menu.html):

**Problemas encontrados:**

1. No has seguido exactamente la lista solicitada:
   - **Pedido:** Café latte, American, Machiatto, Capuccino
   - **Tu lista:** Espresso, Americano, Cappuccino, Latte, Mocha (con sublistas adicionales)

2. Para los tés:
   - **Pedido:** Earl Grey, Green Tea, Rooibos
   - **Tu lista:** Green tea, Black tea, Oolong tea, White tea (con sublistas)

**Observación positiva:** Has demostrado conocimientos avanzados al crear listas anidadas con `<ol>` y `<ul>`, lo cual es excelente. Sin embargo, en este ejercicio se pedía seguir exactamente las listas especificadas.

**Recomendación:** Cuando un ejercicio tiene especificaciones concretas, es importante seguirlas al pie de la letra. Luego, si quieres experimentar, puedes crear una versión adicional con tus propias variaciones.

### Iteración 6 Bonus: Tabla - NO COMPLETADA (0/5 puntos)

No has transformado el menú en una tabla. Para hacerlo, deberías usar las etiquetas `<table>`, `<thead>`, `<tbody>`, `<tr>`, `<th>` y `<td>`.

**Ejemplo de estructura:**

```html
<table>
  <thead>
    <tr>
      <th>Tipo</th>
      <th>Bebida</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Café</td>
      <td>Café latte</td>
    </tr>
    <!-- más filas -->
  </tbody>
</table>
```

### Iteración 7: Formulario de Reservas - PARCIALMENTE COMPLETADA (3/6 puntos)

En tu archivo [contact.html](contact.html):

**Lo que has hecho bien:**

- Has creado un formulario funcional
- Has usado `<label>` para cada campo
- Has añadido validación con `required`
- Has incluido el botón de envío

**Lo que necesita corrección:**

1. **Falta el título:** Las instrucciones pedían un título "Reservas Aquí" (puedes usar `<h2>` o `<h3>`)

2. **Opciones incorrectas:**
   - Pedido: "Snack or Breakfast"
   - Tu formulario: "Producto1, Producto2, Producto3"

   Debería ser:

   ```html
   <label for="meal-type">Tipo de comida:</label>
   <select name="meal-type" id="meal-type">
     <option value="snack">Snack</option>
     <option value="breakfast">Breakfast</option>
   </select>
   ```

3. **Número de comensales:** Has puesto hasta 5, pero las instrucciones especificaban de 1 a 4.

4. **Campos adicionales:** Has añadido campos de email y message que no estaban en las instrucciones. Aunque son útiles en un formulario real, en este ejercicio es importante seguir las especificaciones.

### Iteración 8: Elementos del pie de página - INCOMPLETA (1/4 puntos)

**Lo que falta:**

1. **Link de correo:** Has puesto `<a href="contact.html">Contact us</a>`, pero las instrucciones pedían que el enlace abriera la aplicación de correo del usuario. Para esto debes usar `mailto:`:

   ```html
   <a href="mailto:info@urbantoast.com">Contact us</a>
   ```

2. **Horario de apertura:** No has incluido el horario del restaurante en el footer.

### Bonus: Vídeo - NO COMPLETADA (0/3 puntos)

No has cambiado la imagen por un vídeo. Para hacerlo, necesitarías usar las etiquetas `<video>`, `<source>` y sus atributos como `controls`, `autoplay`, etc.

### Bonus Bonus: CSS - COMPLETADO ✓ (+10 puntos extra)

Has demostrado iniciativa al agregar estilos CSS. Esto es un punto muy positivo que suma a tu nota. Has trabajado con:

- Colores de fondo
- Tipografías
- Flexbox para la navegación
- Alineación de textos

Este es un gran plus que demuestra que estás yendo más allá de lo básico.

## Estructura General y Buenas Prácticas

### Aspectos Positivos:

1. Has creado páginas separadas para cada sección (About Us, Menu, Contact), lo cual es una buena práctica de organización
2. Has usado elementos semánticos HTML5: `<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`, `<figure>`, `<figcaption>`
3. Has vinculado correctamente tu hoja de estilos CSS
4. Has usado el atributo `alt` en la imagen (aunque no se ve en tu código)
5. Tu código está relativamente bien indentado

### Aspectos a Mejorar:

1. **Consistencia en los títulos:** En [index.html](index.html) usas "Urban Toast" pero en las otras páginas "Urban toast" (con 't' minúscula)
2. **Enlaces rotos:** En [Aboutus.html](Aboutus.html) línea 14, el enlace apunta a "about.html" pero el archivo se llama "Aboutus.html"
3. **Doble apertura de DOCTYPE:** En [index.html](index.html) línea 1 tienes `<<!DOCTYPE html>` (doble `<`). Esto es un error de sintaxis
4. **Espacios en el HTML:** Hay algunos espacios inconsistentes en tu código que afectan la legibilidad

## Revisión de Commits

Tus commits personales fueron:

- `del double paragraph`
- `img center`
- `add styles menus`
- `add style and ejercices`

### Sugerencias para Mejorar tus Mensajes de Commit:

**Principios básicos de buenos commits:**

1. **Usa el modo imperativo:** Escribe como si estuvieras dando una orden
   - ❌ Malo: "added styles" o "adding styles"
   - ✓ Bueno: "Add styles to navigation menu"

2. **Sé descriptivo pero conciso:** Explica QUÉ y POR QUÉ (si es necesario), no cómo
   - ❌ Malo: "changes"
   - ✓ Bueno: "Fix navigation links in About Us page"

3. **Primera letra mayúscula, sin punto final:**
   - ❌ Malo: "add styles."
   - ✓ Bueno: "Add styles"

4. **Si el cambio es complejo, añade una descripción:**

   ```
   Add form validation to contact page

   - Add required attribute to name and email fields
   - Add pattern validation for email
   - Update submit button styles
   ```

**Aplicado a tus commits:**

| Tu commit                 | Mejor versión                                    |
| ------------------------- | ------------------------------------------------ |
| `del double paragraph`    | `Fix duplicate paragraph in index page`          |
| `img center`              | `Center hero image on home page`                 |
| `add styles menus`        | `Add CSS styles to menu navigation`              |
| `add style and ejercices` | `Add CSS stylesheet and complete HTML exercises` |

**Recursos recomendados:**

- [Conventional Commits](https://www.conventionalcommits.org/)
- [How to Write a Git Commit Message](https://chris.beams.io/posts/git-commit/)

## Validación W3C

Las instrucciones pedían validar tu código con el W3C Validator. Te recomiendo hacerlo:

1. Ve a https://validator.w3.org/
2. Sube tus archivos HTML o pega el código
3. Corrige los errores que te señale (como el doble `<` en el DOCTYPE)

## Recomendaciones Finales

### Prioridades para Mejorar:

**Alta prioridad (afectan la funcionalidad):**

1. Corregir el error de sintaxis en el DOCTYPE de [index.html](index.html)
2. Arreglar el enlace roto en [Aboutus.html](Aboutus.html)
3. Completar la navegación con HOME y DAILY OFFER
4. Usar `<strong>` en lugar de `<span>` para "quality ingredients"
5. Usar `<blockquote>` en lugar de `<cite>` para la cita
6. Añadir el enlace mailto: en el footer
7. Corregir las opciones del formulario según las especificaciones

**Media prioridad (mejoran la calidad):**

1. Añadir el horario de apertura en el footer
2. Seguir exactamente las listas de bebidas solicitadas
3. Añadir el título al formulario de reservas
4. Mantener consistencia en los títulos de las páginas

**Baja prioridad (extras y bonus):**

1. Crear la tabla del menú
2. Implementar el vídeo en lugar de la imagen

### Recursos para Seguir Aprendiendo:

1. **Elementos semánticos HTML:**
   - [MDN - HTML elements reference](https://developer.mozilla.org/es/docs/Web/HTML/Element)
2. **Formularios:**
   - [MDN - Formularios HTML](https://developer.mozilla.org/es/docs/Learn/Forms)
3. **Tablas:**
   - [MDN - Tablas HTML](https://developer.mozilla.org/es/docs/Learn/HTML/Tables/Basics)

4. **Accesibilidad:**
   - [WebAIM](https://webaim.org/)

## Aspectos Destacables

Quiero enfatizar varios puntos muy positivos de tu trabajo:

1. **Iniciativa:** Has ido más allá al crear múltiples páginas y añadir CSS
2. **Estructura semántica:** Usas correctamente las etiquetas HTML5 semánticas
3. **Organización:** Tu proyecto está bien estructurado en archivos separados
4. **Persistencia:** Se nota que has trabajado y experimentado con el código

Con las correcciones sugeridas y poniendo atención a los detalles de las especificaciones, llevarás tu proyecto al siguiente nivel. Recuerda que en programación, seguir las especificaciones es tan importante como escribir código que funcione.

## Próximos Pasos

1. Lee esta corrección con calma
2. Haz una lista de las correcciones prioritarias
3. Trabaja en ellas una por una
4. Valida tu código con W3C
5. Haz commits descriptivos de cada corrección
6. Si tienes dudas, no dudes en preguntar

Has demostrado que tienes las bases. Ahora es momento de refinar y prestar atención a los detalles. Sigue así.
