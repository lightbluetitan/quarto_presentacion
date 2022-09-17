---
title: "Sintaxis Básica Markdown"
author: "Renzo Cáceres Rossi"
date: "2022/09/10"
subtitle: "Markdown - RMarkdown"
always_allow_html: yes
---

<!-- Añadir comentarios a nuestro documento Markdown -->

[Fin Documento](#def)

<a name="abc"> </a>

# Sintaxis Markdown

**Markdown** es un lenguaje de marcado ligero, siendo **RMarkdown**[^1] uno de sus dialectos, una de sus variantes, uno de sus sabores (**Markdown Flavours**).

## Encabezados - Títulos

# Título 1
## Título 2
### Título 3
#### Título 4
##### Título 5
###### Título 6

Título 1
=========

Título 2
--------

## Separaciones - Línea Horizontal

---

---

***

***


## Citas - Añadir citas a nuestro documento Markdown

> "La tecnología no es nada. Lo importante es que tengas fe en la gente, que sean básicamente buenas e inteligentes, y si les das herramientas, harán cosas maravillosas con ellas."
> Steve Jobs

## Negrita - Cursiva - Tachado - Subrayado

**Texto formateado como Negrita**

*Texto formateado como Cursiva*

~~Texto tachado~~

<u>Texto subrayado</u> <!--HTML Tags-->


## Listas

### Lista Viñetas - Lista Anidada

- Lista 1

- Lista 2

- Lista 3

- Lista 4

- Lista 5
  - Lista 5.1
  - Lista 5.2
  - Lista 5.3
  
- Lista 6

- Lista 7


### Lista Numerada

1. Lista 1
2. Lista 2
3. Lista 3
4. Lista 4
5. Lista 5
6. Lista 6

### Lista Ordenada Alfabeticamente

a. Lista A
b. Lista B
c. Lista C
d. Lista D
e. Lista E
f. Lista F

### Listas

- Lista 1
- Lista 2
- Lista 3
* Lista 4
* Lista 5
* Lista 6
+ Lista 7
+ Lista 8
+ Lista 9


## Tablas - Añadir tablas a nuestro documento Markdown


|TABLA A|TABLA B|TABLA C|
|:-----:|:-----:|:-----:|
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |


## Links - Añadir links a nuestro documento Markdown


<https://hablamosr.blogspot.com/>{target=_blank}

[Hablamos R](https://hablamosr.blogspot.com/){target=_blank}

[Hablamos R](https://hablamosr.blogspot.com/ "Ingresa a Hablamos R"){target=_blank}


## Imágenes - Añadir imágenes a nuestro documento Markdown

<center>

![**Logo R**](logo_r.png)


</center>

## Mapas - Añadir mapas a nuestro documento Markdown

<br>

<center>

<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3901.980822578654!2d-77.03197518561798!3d-12.044840345143056!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x9105c8b5d35662c7%3A0x15f0bda5ccbd31eb!2sPalacio%20de%20Gobierno%20del%20Per%C3%BA!5e0!3m2!1ses!2spe!4v1662817365554!5m2!1ses!2spe" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade" data-external=1></iframe>

</center>


## Vídeos - Añadir vídeos a nuestro documento Markdown

<br>

<center>

<iframe width="560" height="315" src="https://www.youtube.com/embed/EkxRj02iaLk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen data-external=1></iframe>


</center>


## Código - Añadir código a nuestro documento Markdown (R - Python - SQL)

    summary(mtcars)
    
La función `barplot()` nos permite crear diagramas de barras (**Bar Charts**) en el lenguaje de programación R.

```R
x <- table(mtcars$cyl)

colores <- c("orange","blue","purple")

barplot(x,xlab="Cilindros",ylab="Frecuencias",main="Número de Cilindros",col=colores)


```


```Python
import matplotlib.pyplot as plt
 

eje_x = ['Python', 'R', 'Node.js', 'PHP']
 

eje_y = [50,20,35,47]
 

plt.bar(eje_x, eje_y)
 

plt.ylabel('Cantidad de usuarios')
 

plt.xlabel('Lenguajes de programación')
 

plt.title('Usuarios de lenguajes de programación')
 

plt.show()


```

    select id_usuario,usuario_nombre,usuario_apellido from usuarios;
    
```sql
USE Northwind

SELECT * FROM Products

```

## Anular sintaxis Markdown


\**Este texto debería ser formateado como Negrita**


\*Este texto debería ser formateado como Cursiva*


\~~Este texto debería ser tachado~~




[Inicio Documento](#abc)

<a name="def"></a>

## Pie de página

[^1]: **RMarkdown** es un paquete del lenguaje de programación R, que nos permite crear documentos científicos y técnicos, para convertirlos a formatos tales como HTML,PDF,Microsoft Word entre otros.

