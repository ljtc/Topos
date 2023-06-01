---
layout: page
title: El topos de conjuntos
description: >
  Definición del concepto de topos
hide_description: true
sitemap: false
---

En esta sección veremos algunas de las cosas que hacen que un topos se parezca a $$\mathbf{Con}$$. Empezamos haciendo algunas observaciones sobre álgebras de Heyting y qué les hace falta para ser álgebras de Boole. Estas propiedades serán usadas para dar la definición de topos booleano y algunas equivalencias.

### Definición
Un topos es booleano si la estructura de álgebra de Heyting del clasificador de subobjetos es un álgebra de Boole.

### Proiposición
Los siguientes enunciados son equivalentes:
1. $$\mathcal{E}$$ es booleano,
2. $$\neg\neg\colon\Omega\to\Omega$$ es igual a $$id_{\Omega}$$,
3. $$Sub(E)$$ es un álgebra de Boole para cualquier $$E\in\mathcal{E}$$,
4. para cualquier $$S\in Sub(E)$$ se cumple $$S\lor\neg S=E$$,
5. los monos $$v\colon 1\to\Omega$$ y $$f\colon 1\to\Omega$$ induce un iso $$\Omega\cong 1+1$$.

Ahora, dadas una topología de Lawvere-Tierney $$j\colon\Omega\to\Omega$$ en un topos $$\mathcal{E}$$ y una gavilla $$F\in\mathcal{E}_j$$, es posible relacionar las estructuras $$Sub_{\mathcal{E}}(F)$$ con $$Sub_{\mathcal{E}_j}(F)$$. La idea de la comparación es que los elementos de la segunda son subobjetos cerrados de la gavilla $$F$$.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/HooNm3zmtsU" title="Clase61" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

Con lo anterior podemos demostrar que $$\mathcal{E}_{\neg\neg}$$ es un topos booleano. Por esta razón lo llamaremos la *booleanización* de $$\mathcal{E}$$.

Luego, diremos que un topos es bien punteado si $$1$$ es generador. Esta propiedad, que tiene el conjunto $$\{\emptyset\}$$ en $$\mathbf{Con}$$, es suficientemente fuerte para hacer al topos booleano, además de $$2$$-valuado.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/PKRgaPqG3Xs" title="Clase62" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

La última propiedad, que no veremos con detalle, del topos $$\mathbf{Con}$$ que veremos es la existencia de un objeto de números naturales. En este momento sólo veremos cómo interactúa con morfismos geométricos, es decir, un par de funtores adjuntos tales que el izquierdo preserva límites finitos. Gracias a esta interacción será posible demostrar que una gran variedad de topos, al menos todos los de Grothendieck, tienen un objeto de números naturales.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/v-umlyNJb20" title="Clase63" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>