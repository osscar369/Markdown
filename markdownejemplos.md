# SINTAXIS MARKDOWN (h1)
Para los encabezados se utilizan tantas almohadillas como h queramos h1 es #, H es ##, etc
## CABECERAS (h2)
### SUBRAYADO CABECERAS (h3)
Para el subrayado de cabeceras utilizamos:

# Para el h1
=====

## Para el H2
-----

### Subrayados, negritas y cursivas
*Con el signo de multiplicar antes y depués itálica*

_Con los guiones bajos antes y después itálica también_

**Para las negritas dos signos de multiplicar antes y después o dos guiones bajos antes y después**

~~Para el tachado se utilizan dos "virgulillas" antes y después.~~ 
Hay que presionar dos veces la combinación "altGr + 4" para las virgulillas.
### Listas numeradas

Se inicia la lista con el 1. (en el editor, al darle al intro ya aparece el siguiente elemento 2.)
1. elemento uno de la lista numerada
2. elemento 2  de la lista numerada
3. elemento 3 de la lista numerada

### Listas no nuemradas

Nos vale tanto el signo de multiplicar como el de menos o el de más para cada elemento (*-+)

* lista desordenada 
* Otro elemento
* Otro más 

+ Probando con el más
+ No mezclan bien
+ Mejor todos iguales

- Y una con el menos
- De Dos elementos
- Hay que dejar un espacio entre el signo y la primera letra para que funcione

### Listas anidadas

1. una lista
2. Con dos elementos
   1. Le metemos tabulador y crea lista anidada
   2. Con otros dos elementos


* Probamos con una desordenada
  * tabulador y listo
    * incluso funciona en más niveles de lista

### Enlaces

El anchor text va entre corchetes y la url va entre paréntesis. 

[ir a google](https://www.google.com)

Puedes hacer referencia a enlaces de esta forma http://www.example.com o de esta otra <http://www.example.com> 


### Imágenes (directas)

El comando ![alt text](url de la imagen + "Título") Sin espacios entre los corchetes y el paréntesis

Ejemplos 

![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "texto por defecto del logo")

![alt text](https://www.tableau.com/sites/default/files/2021-08/multiple_marks_layer_support.gif "El título al pasar el cursor")

### Imágenes referenciadas

Ver en Word teoría

![alt text][logo]


Otro ejemplo:

![alt text][Google Fotos]

### Imágenes como Tags

Se utiliza la etiqueta img de HTML

<img width="500" src="https://www.purina.es/sites/g/files/mcldtz1656/files/2017-11/Bringing-Your-Kitten-Home_0.jpg">

Otro ejemplo

<img width="300" src="https://estaticos.muyinteresante.es/media/cache/1140x_thumb/uploads/images/gallery/5937e90a5bafe882f5bc09e6/gatitos-cesta_0.jpg">










[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "texto por defecto del logo"


[Google fotos]: https://i.blogs.es/5b560d/google-fotos/450_1000.jpg "Logo de Google fotos"

### Insertar bloques de código en diferentes lenguajes
```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```
 
```python
s = "Python syntax highlighting"
print s
```

```html
<html> 
<body>
    <p>Ir a google</>
    <a href="www.google.es">Ir a google</a>
<body>
</html>
```

```
Sin lenguaje especificado 
But let's throw in a <b>tag</b>.
```
```css
h1{
    background color: black;
}
```
### Tablas

| Izquierda | Centro    | Derecha   |
| --------- |:---------:| --------: |
| angel     | a         | $160      |
| pepe      | b         |   $172    |
| bea        | c         |    $122   |

| Col1 | Col 2| Col 3 | Col 4|
| -----| ---  | ------|---   |
|Hola  | Qué tal| como estás| Hoy|
| 18  | 36 | 54 |  72 |

### Formato en tablas

Markdown | Less | Pretty
--- | --- | ---
*cursiva* | `render` | **negrita**
1 | 2 | 3

### Blocquotes o citas

> El blockquote se usa para escribir una cita textual o un párrafo exacto y que éste se diferencie del resto del texto.
> Esta línea es parte del Blockquotes.

>Otra cita. -Parece que no lleva etiqueta de finalización
 
**Para blockquotes anidados: > y después >>**
> hola, que tal
>> Muy bien gracias

### Líneas horizontales :house:

1
____
2
****
### Menciones

@oscar 

### Lista de tareas

- [x] comprar pan
- [ ] ver pelicula con Paula
- [x] @mentions, #refs, [links](), **formatting**, y <del>tags</del>
- [x] otras tareas

Otro ejemplo

- [x] estudiar Markdown
- [ ] ~~Hacer~~ el **cuestionario** de *entornos*
- [ ] Seguir [con el]() estudio

### Emojis

:house: :smile: :phone:

### Enlace a video de YouTube con imagen como anchor

<a href="http://www.youtube.com/watch?feature=player_embedded&v=TtSWo2nbzAk
" target="_blank">
<img src="http://img.youtube.com/vi/TtSWo2nbzAk/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="5" /></a>

### COLORES

```diff
- esto es rojo
+ esto es verde
# esto gris
! esto es amarillo
```
```diff
-Probando con otro ejemplo
```
```diff
!Me gusta el amarillo

```diff
-<span style="color:red">Angel</span>
```


### Expresiones matemáticas

Puedes rendear con *LaTeX* expresiones matemáticas, usando
 **MathJax**

<script type="text/javascript" src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS_HTML"></script>
$$
\Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt\,.
$$

### Diagramas Mermaid

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

```mermaid
graph TD;
    HTML-->CSS;
    HTML-->JAVASCRIPT;
    CSS-->DIOS;
    JAVASCRIPT-->DIOS;
````

### Diagramas UML

```sequence
Alice->Bob: Hello Bob, how are you?
Note right of Bob: Bob thinks
Bob-->Alice: I am good thanks!
```
```sequence
Oscar->Caro: Hola Caro
Note right of Caro: Caro smiles
Caro--> Oscar: Holi
```
### Diagramas de flujo

```flow
st=>start: Start
e=>end
op=>operation: My Operation
cond=>condition: Yes or No?

st->op->cond
cond(yes)->e
cond(no)->op
```

|Alumno|Materia|Calificación
|:---------|:--------:|--------------:|
|Ana|Mate|7.4|
|Rosa|Ciencias|9.1|
|Juana|Inglés|2.8|

+ [x] Distancia de 2 metros
+ [x] Lavarse las manos frecuentemente
+ [ ] Uso de mascarillas

