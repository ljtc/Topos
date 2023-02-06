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
  (FA'\xrightarrow{f}B)\; \mapsto\; (FA\xrightarrow{Fa}FA'\xrightarrow{f}B)
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

<iframe width="560" height="315" src="https://www.youtube.com/embed/Hgk3--yc_Ig" title="Clase 3" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

