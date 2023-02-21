---
layout: page
title: Adjunciones
description: >
  Este es el primer tema importante del curso
hide_description: true
sitemap: false
---

Durante toda esta parte estaremo usando $$\mathbf{A}$$ y $$\mathbf{B}$$ dos categorías y 
$$F\colon\mathbf{A}\to\mathbf{B}$$ y $$G\colon\mathbf{B}\to\mathbf{A}$$ dos funtores.

## Definición

Decimos que $$F$$ es adjunto izquierdo de $$G$$ (o que $$G$$ es adjunto derecho de $$F$$), denotado con 
$$F\dashv G$$ si para cualesquiera objetos $$A\in\mathbf{A}$$ y $$B\in\mathbf{B}$$ hay una biyección 
natural en $$A$$ y $$B$$

$$
\varphi_{A,B}\colon\mathbf{B}(FA,B)\longrightarrow\mathbf{A}(A,GB)
$$

Para decir qué significa la naturalidad en $$A$$ necesitamos tomar una flecha $$a\colon A\to A'$$
y considerar la siguiente función

$$
\begin{gather*}
  \mathbf{B}(Fa,B)\colon\mathbf{B}(FA',B)\longrightarrow\mathbf{B}(FA,B)\\
  (FA'\xrightarrow{f}B)\quad \mapsto\quad (FA\xrightarrow{Fa}FA'\xrightarrow{f}B)
\end{gather*}
$$

En otras palabras, en la notación de arriba, la función $$\mathbf{B}(Fa,B)$$ "pega" a $$Fa$$ a la izquierda de $$f$$. También hay una función, con definición análoga, $$\mathbf{A}(a,GB)$$.
Con estas funciones la naturalidad de $$\varphi_{A,B}$$ en $$A$$ significa 

$$
\mathbf{A}(a,GB)\varphi_{A,B}=\varphi_{A',B}\mathbf{A}(Fa,B)
$$

Como la definición está escrita en términos de conjuntos y funciones, entonces veremos una equivalencia 
que no use a la categoría $$\mathbf{Con}$$. Para demostrar que nuestra definición implica cualquier 
equivalencia se usa la naturalidad de la biyección de manera conveniente.


## Unidad y Counidad
Si $$F\dashv G$$ entonces podemos tomar $$B=FA$$ en la biyección natural, de esta forma tenemos la biyección

$$
\varphi_{A,FA}\colon\mathbf{B}(FA,FA)\longrightarrow\mathbf{A}(A,GFA).
$$

Como $$\mathbf{B}$$ es una categoría arbitraria, entonces la única flecha que podemos tomar en el dominio de $$\varphi_{A,FA}$$ es la identidad. Así, definimos 

$$
\eta_A=\varphi_{A,FA}(\mathrm{id}_{FA})\colon A\to GFA.
$$

Es posible demostrar que $$\eta_A$$ es la componente en $$A$$ de una transformación natural
$$\eta\colon\mathrm{Id}_{\mathbf{A}} \to GF$$ que llamamos la *unidad de la adjunción*.

Análogamente, si tomamos $$A=GB$$ en la biyección natural original entonces obtenemos

$$
\varphi_{GB,B}\colon\mathbf{B}(FGB,B)\longrightarrow\mathbf{A}(GB,GB).
$$

Ahora, en el codominio sólo podemos asegurar la existencia de la identidad y como $$\varphi_{GB,B}$$ es 
una biyección, entonces debe existir una única flecha en el dominio que vaya a la identidad. Por lo 
tanto, podemos definir $$\varepsilon_B\colon FGB\to B$$ como la flecha que satisface $$\varphi_{GB,B}(\varepsilon_B)=\mathrm{id}_{GB}$$. De la misma manera que con la unidad, estas flechas son parte de una 
tranformación natural $$\varepsilon\colon FG\to\mathrm{Id}_{\mathbf{B}}$$ llamada la *counidad de la adjunción*.

Tanto la unidad como la counidad satisfacen una propiedad univesal. Con esta propiedad será posible demostrar una equivalencia de adjunción, además de poder demostrar la propiedad que eventualmente también será otra equivalencia del concepto de adjunción.

<p> </p>

<iframe width="560" height="315" src="https://www.youtube.com/embed/Hgk3--yc_Ig" title="Clase 3" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


## Identidades triangulares
Usando que las componentes de la unidad y la counidad son flechas universales es posible recuperar la biyección natural de la definición de adjunción. Con la unidad tenemos

$$
\begin{gather*}
  \varphi_{A,B}\mathbf{B}(FA,B)\longrightarrow\mathbf{A}(A,GB)\\
  (FA\xrightarrow{f}B) \quad\mapsto\quad (A\xrightarrow{\eta_A}GFA\xrightarrow{Gf}GB).
\end{gather*}
$$

Mientra que con la counidad podemos definir a la inversa de $$\varphi$$, que denotaremos con $$\psi$$, como sigue

$$
\begin{gather*}
  \psi_{A,B}\mathbf{A}(A,GB)\longrightarrow\mathbf{B}(FA,B)\\
  (A\xrightarrow{g}GB) \quad\mapsto\quad (FA\xrightarrow{Fg}FGB\xrightarrow{\varepsilon_B}B).
\end{gather*}
$$

Ahora, podemos usar estas reglas de evaluación para repetir lo que hicimos para obtener a la unidad (usando a $$\psi$$) y la counidad (mediante $$\varphi$$). De esta forma obtendremos dos ecuaciones que son conocidas como las *identidades triangulares*

<p> </p>

<iframe width="560" height="315" src="https://www.youtube.com/embed/fZZnXU__ShI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


## Ejemplos
Un ejemplo de adjunción se obtiene considerando los funtores que olvidan y los libres. En particular, si 
$$G\colon\mathbf{Gru}\to\mathbf{Con}$$ es el funtor que olvida la estructura de grupo y 
$$F\colon\mathbf{Con}\to\mathbf{Gru}$$ es el funtor que a cada conjunto la asocia su grupo libre, entonces 
$$F\dashv G$$. La unidad en la componente $$X$$ debe ser la función

$$
\begin{gather*}
  \eta_X\colon X\longrightarrow GFX\\
  x\mapsto (x)
\end{gather*}
$$

y la counidad en la componente $$H$$ es el morfismo

$$
\begin{gather}
  \varepsilon_H\colon GFH\to H\\
  (xy^*)\mapsto x\cdot y^{-1}
\end{gather}
$$

No es difícil ver que estas son transformaciones naturales y satisfacen las identidades triangulares. Así, podemos decir que el grupo libre está definido como el adjunto derecho del funtor que olvida. En otras palabras es posible definir grupo libre mediante adjunciones.

<iframe width="560" height="315" src="https://www.youtube.com/embed/GKU-kcMWaHI" title="clase5" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

Otro ejemplo que muestra una característica interesante del poder definitorio que tienen las adjunciones es la oposición que hay entra par e impar en $$(\mathbb{N},\leq)$$. En $$\mathbb{N}$$ son conceptos completamente opuestos (la intersección de los correspondientes subconjuntos es vacía); sin embargo, veremos que están parametrizados por el mismo objeto.

Consideramos las funciones $$2n,2n+1\colon\mathbb{N}\to\mathbb{N}$$. Con la primera obtenemos a los pares y con la segunda a los impares. Además, consideramos la función $$h\colon\mathbb{N}\to\mathbb{N}$$ definida por pedazos

$$
h(m)=
\begin{cases}
m/2 & \text{si } m \text{ es par}\\
(m-1)/2 & \text{si } m \text{ es impar.}
\end{cases}
$$

No es difícil mostrar que las tres funciones preservan el orden, es decir, son funtores de la categoría inducida por el orden parcial $$(\mathbb{N},\leq)$$ en sí misma. Más aún, se satisface $$2n\dashv h\dashv 2n+1$$ y las composiciones $$h\circ 2n$$ y $$ h\circ 2n+1$$ son las identidades. Estas condiciones serán lo que llamaremos unidad e identidad de los opuestos adjuntos.

(Ver el primer vídeo en [el Lema de Yoneda-Grothendieck](./yoneda.md))

Es posible demostrar que si $$F\dashv G$$ $$F\dashv G'$$, entonces $$G\cong G'$$ y algo similar con los adjuntos izquierdos. Además, nos permiten definir conceptos como equivalencia de categorías.

<iframe width="560" height="315" src="https://www.youtube.com/embed/1Vc842ZqgeM" title="Clase7" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

