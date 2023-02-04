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
