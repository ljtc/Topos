---
layout: page
title: Factorización e imagen
description: >
  Definición del concepto de topos
hide_description: true
sitemap: false
---

En la categoría de conjuntos es claro que si tomamos una función $$f\colon A\to B$$ arbitraria entonces podemos considerar 
su imagen $$im(f)\subseteq B$$. Con esta imagen podemos pensar que $$f$$ es una función de $$A$$ en $$im(f)$$, donde $$f$$ 
se vuelve suprayectiva. Así, la función original se escribir como una función suprayectiva seguida de una inclusión

$$
A\xrightarrow{f}im(f)\hookrightarrow B
$$

En esta sección veremos que esta factorización también es posible en un topos y lo haremos formalizando el concepto de 
imagen. Además, la factorización que haremos será funtorial.

En este momento el concepto de imagen nos será de utilidad para lograr que las colecciones de subobjetos $$Sub(B)$$ no sólo sean órdenes parciales, sino retículas. El ínfimo se obtiene con el producto fibrado de subobjetos y el supremo requiere de la imagen para sea un subobjeto de $$B$$.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/L9Q6nU1eG30" title="Clase27" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

Dada una flecha $$k\colon A\to B$$ en $$\mathcal{E}$$ podemos hacer una función $$k^{-1}\colon Sub(B)\to Sub(A)$$ que hace 
imagen inversa (producto fibrado a lo largo de $$k$$). Es fácil ver que esta función es un morfismo de órdenes. En 
realidad será un morfismo de retículas pero para ver que preserva ínfimos y supremos veremos que tiene adjuntos izquierdo 
y derecho.

Ya habíamos visto, cuando $$k$$ es mono, que el adjunto izquierdo es "imagen directa" (en ese contexto fue simplemente 
componer con el mono $$k$$). Ahora que tenemos un concepto de imagen de una flecha podemos repetir las ideas para obtener 
el adjunto izquierdo $$\exists_k\colon Sub(A)\to Sub(B)$$ de $$k^{-1}$$.

Una vez que ya tenemos que $$k^{-1}$$ tiene adjunto izquierdo, entonces debe preservar todos los límites que existan en el dominio. En particular, preserva intersecciones

$$k^{-1}(S\cap T)=k^{-1}(S)\cap k^{-1}(T)$$

La ecuación anterior también nos dice que $$\cap\colon Sub(B)\times Sub(B)\to Sub(B)$$ es natural en $$B$$. Si además usamos que $$Sub(B)\cong\mathcal{E}(B,\Omega)$$ es natural en $$B$$, entonces podemos definir la flecha

$$\bigwedge_B\colon\mathcal{E}(B,\Omega\times\Omega)\longrightarrow\mathcal{E}(B,\Omega)$$

natural en $$B$$.Así, por el lema de Yoneda-Grothendieck, tenemos una flecha $$\land\colon\Omega\times\Omega\to\Omega$$.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/KGjyObmtbmQ" title="Clase28" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

Ahora, podemos repetir lo anterior para notar que $$\cap\colon Sub(X\times B)\times Sub(X\times B)\to Sub(X\times B)$$ es 
natural en $$X$$. Si seguimos lo anterior, la naturalidad en $$X$$ implica que hay una flecha 
$$\land\colon PX\times PX\to PX$$, es decir, una versión interna para $$\cap$$.

Para mostrar que $$Sub(B)$$ tiene una estructura más rica y que puede ser internalizada, necesitamos un resultado importante acerca de categorías rebanada $$\mathcal{E}/B$$ para un objeto $$B$$.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/qs8RFIdrU5w" title="Clase29" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>