# Markdown

![Markdown](./img/markdown.svg "Logo Markdown")

- [Markdown](#markdown)
  - [¿Qué es Markdown?](#qué-es-markdown)
    - [¿Para qué sirve?](#para-qué-sirve)
  - [Encabezados](#encabezados)
  - [Formato de texto](#formato-de-texto)
    - [Negrita](#negrita)
    - [Cursiva](#cursiva)
    - [Negrita y Cursiva](#negrita-y-cursiva)
  - [Listas](#listas)
    - [Listas Ordenadas](#listas-ordenadas)
    - [Listas Desordenadas](#listas-desordenadas)
    - [Listas de tareas](#listas-de-tareas)
    - [Anidación de Listas](#anidación-de-listas)
  - [Código](#código)
    - [Código en línea](#código-en-línea)
  - [Footnotes](#footnotes)
    - [Alertas](#alertas)

## ¿Qué es Markdown?

Markdown es un lenguaje de **marcado ligero** que permite aplicar formato a un texto utilizando caracteres sencillos de teclado.

Fue creado en 2004 por **John Gruber** con una filosofía clara: que el texto sea fácil de escribir y, sobre todo, fácil de leer incluso cuando no está procesado o "renderizado".

### ¿Para qué sirve?

Aunque escribas en texto plano (como en un Bloc de notas), Markdown permite que ese texto se convierta automáticamente en documentos con negritas, listas, imágenes y tablas. Se usa principalmente para:

- **Documentación técnica**: El archivo `README.md` que ves en casi todos los proyectos de GitHub.
- **Blogs y Webs**: Plataformas como `WordPress`, `Ghost` y `Reddit` lo usan.
- **Toma de notas**: Apps como `Obsidian` o `Notion` se basan en él.
- **Foros**: Para dar formato a mensajes de forma rápida.

## Encabezados

Los encabezados (*Títulos y Subtítulos*) en **Markdown**, se crean utilizando la `#` antes del título o subtítulo. Esto es lo mismo que utilizar las etiquetas de `HTML` como `h1` hasta el `h6`, solo que en **Markdown** se debe colocar la `#` correspondientes a cada etiqueta `h` de `HTML`.

~~~md
# Encabezado nivel 1
## Encabezado nivel 2
### Encabezado nivel 3
#### Encabezado nivel 4
##### Encabezado nivel 5
###### Encabezado nivel 6
~~~

## Formato de texto

Los formatos de texto en Markdown son las distintas formas en que puedes resaltar, organizar o estructurar tu contenido.

### Negrita

Para que un texto aparezca en negrita con ***Markdown*** se utilizan dos `**` o dos guiones bajos `__`, ambos deben colocarse al principio y al final del texto que se quiere resaltar.

~~~text
texto en __negrita__
texto en **negrita**
texto en ne__gri__ta
texto en **negr**ita
~~~

texto en **negr**ita

### Cursiva

Para agregar texto en cursiva con **Markdown** se utiliza un solo asterisco `*` o un solo guión bajo `_` tanto al inicio como al final de lo oración que quieres marcar como cursiva.

~~~text
Esto es un *texto en cursiva*.
Esto es un texto parcialmente en cu*rsi*va.
Esto es un _texto en cursiva_.
~~~

Esto es un *texto en cursiva*.  
Esto es un texto parcialmente en cu*rsi*va.  
Esto es un *texto en cursiva*.

### Negrita y Cursiva

Para que en texto esté resaltado tanto en negrita como en cursiva al mismo tiempo debes agregar tres asteriscos `***` o tres guiones bajos `___` antes y después de una palabra o de una frase.

~~~text
Esto es un ***texto en negrita y cursiva***.
Esto es un ___texto en negrita y cursiva___.
Esto es un texto parcialmente en ne***grita y cursi***va.
~~~

Esto es un ***texto en negrita y cursiva***.  
Esto es un ***texto en negrita y cursiva***.  
Esto es un texto parcialmente en ne***grita y cursi***va.

## Listas

En **Markdown** puedes agregar tanto listas ordenadas como no ordenadas. Las listas no ordenadas contienen enlaces que siguen un orden secuencial, mientras que las ordenadas contienen elementos ordenados arbitrariamente.

### Listas Ordenadas

Para agregar listas ordenadas en **Markdown** se debe agregar un número seguido de un punto `1.`, un espacio y el elemento de la lista. La lista no debe estar ordenada numéricamente, pero debe comenzar por el número `1`.

~~~text
1. Primer elemento
2. Segundo elemento
3. Tercer elemento
~~~

1. Primer elemento
2. Segundo elemento
3. Tercer elemento

### Listas Desordenadas

Para agregar listas no ordenadas en **Markdown** se debe agregar un guion `-`, un signo más `+` o un asterisco `*` delante de los elementos de la lista.

~~~text
- Primer elemento
+ Segundo elemento
* Tercer elemento
~~~

- Primer elemento
+ Segundo elemento
* Tercer elemento

### Listas de tareas

También podemos crear `listas de tareas`, para crear una lista de tareas, se debe añadir como prefijo un guión y espacio, seguido de `[]` a los elementos de la lista. Para marcar una tarea como completada, usamos `[X]`.

~~~text
- [X] Tarea terminada
- [ ] Tarea pendiente
- [ ] Otra tarea por hacer
~~~

- [X] Tarea terminada
- [ ] Tarea pendiente
- [ ] Otra tarea por hacer

### Anidación de Listas

Puedes anidar las listas de diferentes tipos, incluyendo listas dentro de otras listas, ya sean ordenadas o no ordenadas. Para ello, los elementos de la lista anidada tendrán que tener una sangría de al menos cuatro espacios o una tabulación.

~~~text
1. Primer elemento
2. Segundo elemento
    1. Elemento 2 1
    2. Elemento 2 2
3. Tercer elemento
~~~

1. Primer elemento
2. Segundo elemento
   1. Elemento 2 1
   2. Elemento 2 2
3. Tercer elemento

~~~text
* Primer elemento
* Segundo elemento
    * Elemento 2 1
    * Elemento 2 2
* Tercer elemento
~~~

- Primer elemento
- Segundo elemento
  - Elemento 2 1
  - Elemento 2 2
- Tercer elemento

## Código

En **Markdown** también puedes definir bloques de código, tanto en línea como en forma de bloque.

### Código en línea

Para agregar código en línea en **Markdown** usa comillas invertidas ` `` ` alrededor del texto que quieres que tengo formato de código, por ejemplo:

~~~text
Use `git status` para listar todos los archivos nuevos o modificados que aún no se han confirmado.
~~~

Y se vería: Use `git status` para listar todos los archivos nuevos o modificados que aún no se han confirmado.

Para dar formato al código o al texto en su propio bloque diferenciado, use tres comillas invertidas ` ``` ` o tres virgulillas `~~~`.

~~~text
Para insertar las comillas invertidas, puedes utilizar Alt+96
Para insertar las virgulillas, puedes utilizar Alt+126 
~~~

Podemos agregar un identificador opcional de idioma para habilitar el resaltado de la sintaxis en tu bloque de código cercado.

El resaltado de sintaxis cambia el color y el estilo del código fuente para facilitar la lectura.

~~~text
Después de las 3 primeras ~ podemos resaltar la sintaxis del código:

```js
function sumar (a, b) {
    return a + b;
}
```
~~~

El siguiente es un código Javascript:

~~~js
function sumar (a, b) {
    return a + b;
}
~~~

## Footnotes

Podemos agregar notas al pie al contenido mediante esta sintaxis de corchetes `{}`:

~~~text
Aquí hay una nota al pie simple[^1]. 
Una nota al pie también puede tener varias líneas[^2]. 

[^1]: Mi referencia. 
[^2]: Para agregar saltos de línea dentro de una nota al pie, agregue 2 espacios al final de una línea.
Esta es una segunda línea.
~~~

Aquí hay una nota al pie simple [^1].  
Una nota al pie también puede tener varias líneas[^2].  

[^1]: Mi referencia.  
[^2]: Para agregar saltos de línea dentro de una nota al pie, agregue 2 espacios al final de una línea.  
Esta es una segunda línea.

>[!NOTE]
>La posición de una nota al pie en Markdown no influye en dónde se mostrará la nota al pie. Puede escribir una nota al pie justo después de la referencia a dicha nota, y la nota al pie se seguirá mostrando en la parte inferior del documento `Markdown`. Las notas al pie no se admiten en wikis.

### Alertas

**Las alertas**, también conocidas como **llamadas**, **admoniciones** o **advertencias**, son una extensión de Markdown basada en la sintaxis blockquote que puede usar para resaltar la información crítica. En GitHub, se muestran con colores e iconos distintivos para indicar la importancia del contenido.

Use alertas solo cuando sean cruciales para el éxito del usuario y limite a uno o dos por artículo para evitar sobrecargar el lector. Además, debe evitar colocar alertas consecutivamente. Las alertas no se pueden anidar dentro de otros elementos.

Para agregar una alerta, use una línea blockquote `>` especial que especifique el tipo de alerta, seguido de la información de alerta en un blockquote estándar. Hay cinco tipos de alertas disponibles:

~~~text
> [!NOTE]
> Información útil que los usuarios deberían conocer, incluso al hojear el contenido.

> [!TIP]
> Consejos útiles para hacer las cosas mejor o más fácilmente.

> [!IMPORTANT]
> Información clave que los usuarios necesitan saber para lograr su objetivo.

> [!WARNING]
> Información urgente que requiere la atención inmediata del usuario para evitar problemas.

> [!CAUTION]
> Advierte sobre los riesgos o las consecuencias negativas de ciertas acciones.
~~~

> [!NOTE]
> Información útil que los usuarios deberían conocer, incluso al hojear el contenido.
---
> [!TIP]
> Consejos útiles para hacer las cosas mejor o más fácilmente.
---
> [!IMPORTANT]
> Información clave que los usuarios necesitan saber para lograr su objetivo.
---
> [!WARNING]
> Información urgente que requiere la atención inmediata del usuario para evitar problemas.
---
> [!CAUTION]
> Advierte sobre los riesgos o las consecuencias negativas de ciertas acciones.
