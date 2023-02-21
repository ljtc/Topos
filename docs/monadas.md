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


## Toda adjunción induce una mónada





<iframe width="560" height="315" src="https://www.youtube.com/embed/gCDeCJsGDpg" title="Clase9" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>