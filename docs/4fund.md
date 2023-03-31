---
layout: page
title: La categoría rebanada como un topos
description: >
  Definición del concepto de topos
hide_description: true
sitemap: false
---

El objetivo ahora es demostrar el siguiente resultado.

### Teorema (fundamental de la teoría de topos)
Si $$\mathcal{E}$$ es una topos y $$B\in\mathcal{E}$$, entonces $$\mathcal{E}/B$$ es un topos.

Mostrar que tiene límites finitos no es difícil. Por ejemplo, el objeto terminal de $$\mathcal{E}/B$$ es la identidad 
$$B\to B$$ (esta es la razón por la cual muchos autores denotan con $$1_B$$ a la identidad). También es fácil ver que 
$$\mathcal{E}/B$$ tiene productos, ya que estos son productos fibrados en $$\mathcal{E}$$. Los igualadores en 
$$\mathcal{E}/B$$ son igualadores en $$\mathcal{E}$$. Por lo tanto, $$\mathcal{E}/B$$ tiene límites finitos.

El clasificador de subobjetos en $$\mathcal{E}/B$$ se debe construir a partir del clasificador de subobjetos del topos $$\mathcal{E}$$. Así, si tomamos $$\Omega\in\mathcal{E}$$ y queremos obtener un objeto con una flecha hacia $$B$$, lo más fácil es considerar $$p_2\colon\Omega\times B\to B$$. De hecho se demuestra que la proyección anterior es el clasificador de subobjetos en $$\mathcal{E}/B$$.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/9UMYx25AtMM" title="Clase31" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

Ahora sólo falta ver que $$\mathcal{E}/B$$ tiene objetos potencia. Lo primero que haremos para demostrar este hecho es notar que el axioma de objetos potencia es equivalente a que haya una biyección

$$\mathcal{E}(A\times C,\Omega)\cong\mathcal{E}(C,PA)$$

natural en $$A$$ y $$C$$. Así, para cada $$f\colon C\to B$$ en $$\mathcal{E}/B$$ encontraremos un objeto, que denotaremos $$P_B f$$ tal que para cualquier $$g\colon D\to B$$ haya una biyección

$$
\begin{equation}
\mathcal{E}/B(C\times_B D,\Omega\times B)\cong\mathcal{E}/B(D,P_B f)
\end{equation}
$$

natural en $$C$$ y $$D$$.

Empezamos analizando el lado izquierdo de la biyección que queremos, para esto primero daremos una forma conveniente de la 
característica de $$C\times_B D$$ como subobjeto de $$C\times D$$. Además, notamos que una flecha 
$$C\times_B D\to\Omega\times B$$ en $$\mathcal{E}/B$$ está en correspondencia con una flecha $$C\times_B D\to\Omega&& en 
$$\mathcal{E}$$ y esta con un subobjeto de $$C\times_B D$$, que a su vez es lo mismo que un subobjeto de $$C\times D$$ 
contenido en $$C\times_B D$$.