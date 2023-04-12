---
layout: page
title: Objetos retícula y álgebra de Heyting en un topos
description: >
  Definición del concepto de topos
hide_description: true
sitemap: false
---

Empezamos esta sección describiendo quiénes serán los objetos que queremos encontrar de manera interna en un topos.

### Definición
Una retícula es una categoría de orden parcial finitamente completa y cocompleta.

### Definición
Un álgebra de Heyting es una retícula cartesianamente cerrada, es decir, el producto tiene adjunto derecho.

En una categoría en general el adjunto izquierdo del producto se denota con una exponencial. En el caso de categorías de 
orden parcial es común denotar a este adjunto derecho con una implicación. Así, si $$H$$ es un álgebra de Heyting, 
entonces la biyección de "flechas" que define la adjunción es

$$
\begin{array}{c}
a\land b\leq c\\
\hline
b\leq (a\Rightarrow c)
\end{array}
$$

El ejemplo canónico de un álgebra de Heyting es la categoría generada por los abiertos de un espacio topológico ordenados 
con la contención. Otro ejemplo, con el cual podemos explicar la notación de la exponencial en este contexto, es 
considerar formulas proposicionales y ordenarlas como $$\alpha\leq\beta\iff \alpha\vdash\beta$$ si queremos hacer un 
álgebra a partir de la sintaxis, o bien, $$\alpha\leq\beta\iff \alpha\vDash\beta$$ si preferimos la semántica. 
Desgraciadamente esta relación no satisface la antisimetría, así que no ordena parcialmente al conjunto de fórmulas (que 
denotaremos $$Form$$). Esto nos obliga a hacer un cociente módulo la relación de ser lógicamente equivalente. Así, 
$$(Form/\equiv,\leq)$$ es un orden parcial.

El orden parcial $$(Form/\equiv,\leq)$$ tiene la estructura que nos interesa, ya que la conjunción induce un ínfimo 
(producto), la disyunción un supremo (coproducto), la clase de una tautología es el máximo (terminal) y la clase de una 
contradicción es el mínimo (inicial). Con esto tenemos que nuestro orden parcial es de hecho una retícula. Más aún, si 
escribimos la relación que define a la implicación desde el punto de vista sintáctico obtenemos

$$
a\land b\vdash c \iff b\vdash(a\Righarrow c)
$$

Esta relación, en lógica de proposiciones, se conoce como el teorema de la deducción. Así, el teorema de la deducción afirma que $$(Form/\equiv,\leq)$$ es cartesiana cerrada. Así, es un álgebra de Heyting.

La unidad y la counidad de la adjunción también se interpretan como relaciones conocidas en lógica de proposiciones. La unidad es una forma de expresar al primer axioma del cálculo de proposiciones de Mendelson y la counidad es el *modus ponens*.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/IvSG0WNIb_s" title="Clase40" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>