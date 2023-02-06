---
layout: page
title: Grupo libre
description: >
  Esto nos servira para construir muchos ejemplos
hide_description: true
sitemap: false
---

## Funtores que olvidan
Como una estructura está definida como un conjunto con (posiblemente) operaciones, elementos distinguidos y relaciones, entonces siempre podemos olvidarnos de la estructura y quedarnos simplemente con el conjunto subyacente. Además, los morfimos de estructuras son funciones entre los conjuntos subyacentes que preservan la estructura (preservar debe ser entendido en un sentido más ampio ya que las funciones continuas no preservan a los abiertos, la correspondiente noción de estructura, sino que más bien los reflejan). Por lo tanto, también es posible olvidar que un morfismo preserva estructura y quedarse simplemente con una función.

Un ejemplo concreto de un funtor que olvida es $$G\colon\mathbf{Gru}\to\mathbf{Con}$$ que a un morfismo de grupos $$f\colon(H_1,\cdot_1,e_1)\to(H_2,\cdot_2,e_2)$$ lo manda a la función entre los conjuntos subyacentes $$f\colon H_1\to H_2$$.


## Grupos libres
Un tipo de estructura donde no es tan difícil construir la estructura libre generada por un conjunto es en grupos. Dado un conjunto $$X$$ se introduce una copia de cada elemento de $$X$$ para que funcione como su inverso, $$X^*=\{x^*\mid x\in X\}$$. Luego, se consideran las palabras con alfabeto $$X\cup X^*$$, es decir,

$$
\bigcup_{n\in\mathbb{N}}(X\cup X^*)^n .
$$

Finalmente, se toma una relación que forzará a que $$x^*$$ sea el inverso de $$x$$,

$$
x_1\ldots x_i xx^* x_{i+1}\ldots x_n\sim x_1\ldots x_i x_{i+1}\ldots x_n.
$$

(También se pueden eliminar si aparecen en el otro orden, $$x^* x$$.)
Con esto tenemos el conjunto subyacente del que será el grupo libre generado por $$X$$. La multiplicación es la concatenación de palabras y el neutro es la palabra vacía, comúnmente denorada con $$\Lambda$$.

Se puede demostrar que el grupo libre tiene una propiedad universal y que con ella se puede definir en funciones de tal forma que resulte ser un funtor.


<iframe width="560" height="315" src="https://www.youtube.com/embed/T_ZyD91OFr0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
