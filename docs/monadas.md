---
layout: page
title: Mónadas
description: >
  Exploraremos una relación entre adjunciones y ciertos conceptos algebraicos
hide_description: true
sitemap: false
---

## Definición
Una *mónada* es una terna $$(T,\eta,\mu)$$ donde $$T\colon\mathbf{A}\to\mathbf{A}$$ es un funtor, 
$$\eta\colon Id_{\mathbf{A}}\to GF$$ y $$\mu\colon FG\to Id_{\mathbf{A}}$$ son transformaciones naturales. $$\eta$$ es la 
*unidad* y $$\mu$$ es la *multiplicación* de la mónada. Estas transformaciones deben satisfacer la versión diagramática de 
que $$\mu$$ es asociativa y $$\eta$$ es neutro para $$\mu$$.

El tema de mónadas es bastante extenso y profundo, además de tener aplicaciones en otras áreas, como computación. Sin 
embargo, aquí sólo veremos que toda adjunción induce una mónada y viceversa, toda mónada induce una adjunción.


## Toda adjunción induce una mónada
Podemos dar un conjunto de ejemplos de mónadas y al mismo tiempo dar un resultado de utilidad para lo que queremos mostrando que como inducir na mónada mediante una adjunción.

Dada una adjunción $$(F,G,\eta,\mu)\colon\mathbf{A}\to\mathbf{B}$$, definimos una mónada sobre $$\mathbf{A}$$ como sigue: el endofuntor es $$GF$$, la unidad de la mónada es $$\eta$$ y la multiplicación es $$G\varepsilon_F$$. Es fácil ver que lo anterior define mónada.

<iframe width="560" height="315" src="https://www.youtube.com/embed/gCDeCJsGDpg" title="Clase9" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


## Toda mónada induce una adjunción
Para definir una adjunción, dada una mónada $$(T,\eta,\mu)$$ es necesario definir una categoría y dos funtores. 

Una $$T$$-álgebra es una pareja $$(A,h)$$, donde $$A\in\mathbf{A}$$ y $$h\colon TA\to A$$, que satisface la versión 
diagramática que dice $$h$$ es una acción de la mónada $$T$$ en el objeto $$A$$. Si $$(A,h)$$ y $$(A',h')$$ son 
$$T$$-álgebras, entonces un morfismo de $$T$$-álgebras es una flecha $$a\colon A\to A'$$ en $$\mathbf{A}$$ tal que 
$$h\, Th=h\,\mu_A$$.

Es fácil ver que la composición de morfismos de $$T$$-algebras es un morfismo de $$T$$-álgebras y que la identidad también
es un morfismo de $$T$$-álgebras. Así, tenemos una categoría $$\mathbf{A}^T$$ de $$T$$-algebras y morfismos entre ellas.

Por la definición de $$T$$-álgebra y morfismo, no es difícil ver que hay un funtor que se olvida de la estructura de 
$$T$$-álgebra, $$G^T\colon\mathbf{A}^T \to\mathbf{A}$$,

$$
\begin{array}{ccc}
(A,h)       &         & A\\
a\downarrow & \mapsto & \downarrow a\\
(A',h')     &         & A'
\end{array}
$$

Por otro lado, dado un objeto $$A$$ es posible definir una $$T$$-álgebra libre generada por $$A$$. No es difícil mostrar que $$(TA,\mu_A)$$ es una $$T$$-álgebra. Además, si $$a\colon A\to A'$$ entonces $$Ta$$ es un morfismo de $$T$$-álgebras. Así, tenemos un funtor libre $$F^T\colon\mathbf{A}\to\mathbf{A}^T$$. 

$$
\begin{array}{ccc}
A           &         & (TA,\mu_A)\\
a\downarrow & \mapsto & \downarrow Ta\\
A           &         & (TA',\mu_{A'})
\end{array}
$$

Los dos funtores de arriba definen una adjunción $$F^T\dashv G^T$$.


## El funtor de comparación
Si empezamos con una adjunción $$(F,G,\eta,\mu)\colon\mathbf{A}\to\mathbf{B}$$, luego hacemos la mónada inducida 
$$(T,\eta,\mu)$$ y después la adjunción generada por esta mónada $$(F^T,G^T,\eta^T,\mu^T)$$, entonces podemos preguntarnos si hay una relación entre la adjunción con la que empezamos y la con la que terminamos.

El funtor de comparación $$K\colon\mathbf{B}\to\mathbf{B}^T$$ está definido mediante

$$
\begin{array}{ccc}
B           &         & (GB,G\varepsilon_B)\\
b\downarrow & \mapsto & \downarrow Gb\\
B'          &         & (GB,G\varepsilon_{B'})
\end{array}
$$

Este funtor de cierta forma mide que tan algebraica es la categoría $$\mathbf{B}$$ sobre $$\mathbf{A}$$, de tal forma que si resulta se runa equivalencia entonces diremos que $$\mathbf{B}$$ es muy algebraica sobre $$\mathbf{A}$$.
