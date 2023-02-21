---
layout: page
title: Lema de Yoneda-Grothendieck
description: >
  En principio es algo separado de los temas, pero será útil en muchos lugares
hide_description: true
sitemap: false
---

En toda esta sección estaremos usando una categoría pequeña $$\mathbf{C}$$, es decir, tiene un conjunto de objetos y un 
conjunto de flechas. Esta hipótesis es sólo para que no haya problemas de tamaño. Como queremos que $$\mathbf{C}(A,B)$$ 
este en una categoría de conjuntos, lo más fácil es pedir una restricción a $$\mathbf{C}$$ para evitar problemas con ZFC.

## Un pequeño preámbulo
Dado $$C\in\mathbf{C}$$ podemos dar un funtor contravariante $$\mathbf{C}(-,C)\colon\mathbf{C}\to\mathbf{Con}$$.
La evaluación en objetos se puede deducir de la notación, a un objeto $$A\in\mathbf{C}$$ se le asigna el conjunto 
de flechas $$\mathbf{C}(A,C)$$. Si $$f\colon A\to B$$ entonces podemos definir una función

$$
\begin{gather*}
  \mathbf{C}(f,C)\colon \mathbf{C}(B,C)\longrightarrow\mathbf{C}(A,C)\\
  (B\xrightarrow{g}C)\mapsto (A\mapsto{f}B\mapsto{g}C)
\end{gather*}
$$

Estos funtores son objetos en una categoría de funtores $$\mathbf{Con}^{\mathbf{C}^{\text{op}}}$$ que es llamada 
*categoría de pregavillas*. Cada funtor contravariante de $$\mathbf{C}$$ a $$\mathbf{Con}$$ será llamado *pregavilla* y una 
pregavilla es *representable* si es isomorfa a $$\mathbf{C}(-,C)$$ para algún $$C\in\mathbf{C}$$.

## Lema
Si $$C\in\mathbf{C}$$ y $$P\in\mathbf{Con}^{\mathbf{C}^{\text{op}}}$$, entonces hay una biyección

$$
PC\cong \mathbf{Con}^{\mathbf{C}^{\text{op}}}(\mathbf{C}(-,C),P)
$$

<iframe width="560" height="315" src="https://www.youtube.com/embed/9CB2eyuJgJk" title="Clase6" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Una consecuencia
El lema de Yoneda-Grothendieck tiene muchas consecuencias muy útiles en teoría de topos; sin embargo, ahora sólo veremos
una que no depende de ninguna clase de objetos, como topos.

Para enunciar la consecuencia que queremos necesitamos dar un funtor 
$$\mathbf{y}\colon\mathbf{C}\to\mathbf{Con}^{\mathbf{C}^{\text{op}}}$$ definido como $$\mathbf{y}C=\mathbf{C}(-,C)$$. No es difícil ver que este es un funtor covariante. Así, el resultado que nos interesa es

## Corolario
El funtor de Yoneda es fiel y pleno.




