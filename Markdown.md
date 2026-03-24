# Markdown

<div alingn="text-center">
<img src="./img/markdown.svg" style="background-color: #fff" 

<!-- ![Markdown](./img/markdown.svg "Logo Markdown") -->

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
    - [Anidación de Listas](#anidación-de-listas)
  - [Código](#código)
    - [Código en línea](#código-en-línea)

## ¿Qué es Markdown?

Markdown es un lenguaje de **marcado ligero** que permite aplicar formato a un texto utilizando caracteres sencillos de teclado.

Fue creado en 2004 por **John Gruber** con una filosofía clara: que el texto sea fácil de escribir y, sobre todo, fácil de leer incluso cuando no está procesado o "renderizado".

### ¿Para qué sirve?

Aunque escribas en texto plano (como en un Bloc de notas), Markdown permite que ese texto se convierta automáticamente en documentos con negritas, listas, imágenes y tablas. Se usa principalmente para:

- **Documentación técnica**: El archivo ``README.md`` que ves en casi todos los proyectos de GitHub.
- **Blogs y Webs**: Plataformas como ``WordPress``, ``Ghost`` y ``Reddit`` lo usan.
- **Toma de notas**: Apps como ``Obsidian`` o ``Notion`` se basan en él.
- **Foros**: Para dar formato a mensajes de forma rápida.

---

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

    texto en __negrita__
    texto en **negrita**
    texto en ne__gri__ta
    texto en **negr**ita

texto en __negrita__
texto en **negrita**
texto en **negr**ita

### Cursiva

Para agregar texto en cursiva con __Markdown__ se utiliza un solo asterisco `*` o un solo guión bajo `_` tanto al inicio como al final de lo oración que quieres marcar como cursiva.

    Esto es un *texto en cursiva*.
    Esto es un texto parcialmente en cu*rsi*va.
    Esto es un _texto en cursiva_.

Esto es un *texto en cursiva*.
Esto es un texto parcialmente en cu*rsi*va.
Esto es un _texto en cursiva_.

### Negrita y Cursiva

Para que en texto esté resaltado tanto en negrita como en cursiva al mismo tiempo debes agregar tres asteriscos `***` o tres guiones bajos `___` antes y después de una palabra o de una frase.

    Esto es un ***texto en negrita y cursiva***.
    Esto es un ___texto en negrita y cursiva___.
    Esto es un texto parcialmente en ne***grita y cursi***va.

Esto es un ***texto en negrita y cursiva***.
Esto es un ___texto en negrita y cursiva___.
Esto es un texto parcialmente en ne***grita y cursi***va.

## Listas

En **Markdown** puedes agregar tanto listas ordenadas como no ordenadas. Las listas no ordenadas contienen enlaces que siguen un orden secuencial, mientras que las ordenadas contienen elementos ordenados arbitrariamente.

### Listas Ordenadas

Para agregar listas ordenadas en **Markdown** se debe agregar un número seguido de un punto `1.`, un espacio y el elemento de la lista. La lista no debe estar ordenada numéricamente, pero debe comenzar por el número `1`.

    1. Primer elemento
    2. Segundo elemento
    3. Tercer elemento

1. Primer elemento
2. Segundo elemento
3. Tercer elemento

### Listas Desordenadas

Para agregar listas no ordenadas en **Markdown** se debe agregar un guion `-`, un signo más `+` o un asterisco `*` delante de los elementos de la lista.

    - Primer elemento
    + Segundo elemento
    * Tercer elemento

- Primer elemento
+ Segundo elemento
* Tercer elemento

### Anidación de Listas

Puedes anidar las listas de diferentes tipos, incluyendo listas dentro de otras listas, ya sean ordenadas o no ordenadas. Para ello, los elementos de la lista anidada tendrán que tener una sangría de al menos cuatro espacios o una tabulación.

    1. Primer elemento
    2. Segundo elemento
        1. Elemento 2 1
        2. Elemento 2 2
    3. Tercer elemento

1. Primer elemento
2. Segundo elemento
   1. Elemento 2 1
   2. Elemento 2 2
3. Tercer elemento

---
    * Primer elemento
    * Segundo elemento
        * Elemento 2 1
        * Elemento 2 2
    * Tercer elemento

* Primer elemento
* Segundo elemento
    * Elemento 2 1
    * Elemento 2 2
* Tercer elemento

## Código

En **Markdown** también puedes definir bloques de código, tanto en línea como en forma de bloque.

### Código en línea

Para agregar código en línea en **Markdown** usa comillas invertidas ` `` ` alrededor del texto que quieres que tengo formato de código.

    Cambia de directorio con el comando `cd`