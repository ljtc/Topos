---
layout: page
title: Funtor gavilla asociada
description: >
  Definición del concepto de topos
hide_description: true
sitemap: false
---

En esta sección veremos que la inclusión $$\mathcal{E}_j\to\mathcal{E}$$ tiene un adjunto izquierdo que preserva límites 
finitos. La demostración se hará en dos pasos, primero veremos que la inclusión $$Sep_j\mathcal{E}\to\mathcal{E}$$ tiene 
adjunto izquierdo y luego veremos lo correspondiente con la inclusión $$\mathcal{E}_j\to Sep_j\mathcal{E}$$.

Como los objetos separados tienen un papel central en esta sección, empezamos viendo algunas equivalencias de ser 
separado. Más específicamente, los siguientes enunciados son equivalentes:
1. $$C$$ es separado;
2. la diagonal, $$\Delta_C\colon C\to C\times C$$ es cerrada;
3. $$j^C \{\,\}_C=\{\,\}_C$$;
4. Para cualquier flecha $$f\colon A\to C$$, la gráfica de $$f$$ es un subobjeto cerrado de $$A\times C$$.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/0PFNr0_S41A" title="Clase55" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

Ahora empezamos a construir un funtor $$\mathcal{E}\to Sep_j\mathcal{E}$$. Para cada $$E\in\mathcal{E}$$ consideramos la 
composición $$r^E \{\,\}_E$$ y su factorización epi-mono. Si $$\theta_E\colon E\to E'$$ es el epi de la factorización 
anterior, entonces podemos demostrar que $$E'$$ es un objeto separado. Con esto podemos definir la asignación en objetos 
del funtor anterior, $$E\mapsto E'$$. Para demostrar que $$E'$$ es separado se observa que $$\Omega_{j}^{E}$$ es una 
gavilla inyectiva y como tenemos un mono $$E'\rightarrowtail \Omega_{j}^{E}$$ de la factorización epi-mono, entonces 
$$E'$$ es separado, como queríamos.

Una propiedad más acerca de la construcción del epi $$\theta_E\colon E\to E'$$ del párrafo anterior es que si $$E$$ es separado, entonces $$\theta_E$$ es iso. Así, concluimos que $$E$$ es separado si y sólo si $$E$$ se puede encajar en una gavilla inyectiva $$E\rightarrowtail I_E$$.

Finalmente, veremos que el par núcleo del epi $$\theta_E\colon E\to E'$$ es la cerradura de la diagonal.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/uaVmzuq4-OY" title="Clase56" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

Una vez que hemos demostrado lo anterior y recordamos que todo epi es el coigualador de su par núcleo, entonces obtenemos 
que $$\theta_E$$ es el coigualador de la cerradure de la diagonal. Con este coigualador podemos demostrara que 
$$\theta_E$$ es universal respecto a objetos separados, es decir, si $$S$$ es separado y $$f\colon E\to S$$ es una flecha 
arbitraria, entonces existe una única $$G\colon E'\to S$$ tal que $$g\theta_E =f$$.

Ahora que ya sabemos que $$\theta_E$$ es universal respecto a objetos separados podemos definir un funtor

$$
(\,)'\colon \mathcal{E}\to Sep_j \mathcal{E}
$$

de tal forma que $$\theta\colon id_{\mathcal{E}} \to i(\,)'$$ (donde $$i\colon Sep_j\mathcal{E}\to \mathcal{E}$$ es la 
inclusión) sea una transformación natural con componentes $$\theta_E\colon E\to E'$$ definidas como arriba. Además, la 
universalidad respecto a objetos separados muestra que $$\theta$$ es la unidad para la adjunción $$()'\dashv i$$.

<iframe width="560" height="315" src="https://www.youtube.com/embed/lNsQsmV3vak" title="Clase57" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

Para encontrar el adjunto izquierdo de la inclusión $$i\colon\mathcal{E}_j\to Sep_j\mathcal{E}$$, notamos que, en nuestra 
construcción anterior, cuando $$E$$ es separado se tiene que $$\theta_E$$ es iso. Así, hay un mono del separado $$E$$ a un 
gavilla inyectiva $$I_E$$. Luego, sabemos que un subobjeto de una gavilla es gavilla si y sólo sí es cerrado. Por lo 
tanto, al separado $$E$$ le asignamos la gavilla $$\overline{E}\rightarrowtail I_E$$.

Si denotamos con $$\sigma_E\colon E\to I_E$$ al mono que se obtiene con $$E$$ separado e $$I_E$$ gavilla inyectiva, entonces es posible demostrar que $$\sigma_E$$ es universal respecto a gavillas. Como antes, esto implica que podemos dar un funtor

$$
\overline{(\,)}\colon Sep_j\mathcal{E}\to\mathcal{E}_j
$$

de tal forma que $$\sigma$$ es la unidad de la adjunción $$\overline{(\,)}\dashv i$$.

Resumiendo, dado un objeto $$E\in\mathcal{E}$$ podemos encontrar una gavilla inyectiva $$I_E$$ y una flecha 
$$i_E\colon\to I_E$$ con par núcleo mínimo, es decir, el par núcleo de la flecha es la cerradura de la diagonal, 
$$\overline{\Delta_E}$$. Luego, hacemos la factorización epi-mono de la flecha $$i_E$$ para obtener la imagen $$i_E(E)$$. Finalmente, tomamos la cerradura de la imagen, $$\overline{i_E(E)}$$ como subobjetos de $$I_E$$. Esta cerradura es la gavilla asociada al objeto $$E$$ y la denotaremos $$\mathtt{a}E$$. La correspondencia de flechas se por medio de la universalidad de los dos pasos de la construcción. Con esto tenemos el funtor *gavilla asociada*

$$
\mathtt{a}\colon\mathcal{E}\to\mathcal{E}_j
$$

Por la unicidad de los adjuntos, $$\mathtt{a}$$ es adjunto izquierdo de la inclusión 
$$i\colon\mathcal{E}_j\to\mathcal{E}$$. Por último veremos que $$\mathtt{a}$$ preserva límites finitos.

Es fácil ver que $$\mathtt{a}$$ preserva a $$1$$, pues este último es una gavilla. Además, también preserva monos.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/x0DOMA2tYPc" title="Clase58" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

Para demostrar que $$\mathtt{a}$$ preserva productos finitos necesitamos demostrar que 
$$\overline{A\times B}=\overline{A}\times\overline{B}$$, para cualesquiera $$A,B\in Sub(E)$$. Con esta propiedad 
construimos $$\mathtt{a}(E\times F)$$ a partir de la gavilla inyectiva $$I_E\times I_F$$.

La demostración de que $$\mathtt{a}$$ preserva igualadores es un poco más compleja. La idea es tomar un igualador en 
$$\mathcal{E}$$ de la forma $$E\rightarrowtail A\rightrightarrows B$$ y hacer la construcción de la gavilla asociada a 
$$E$$ como en la preservación de monos. Para demostrar que el resultado es el igualador de mandar a las flechas paralelas 
con el funtor $$\mathtt{a}$$, es necesario considerar al igualador de dicho par de flechas y mostrar que es isomorfo a 
$$\mathtt{a}E$$ construido como se menciona. Este isomorfismo se construye viendo que los objetos en cuestión se contienen 
mutuamente respecto a $$\mathtt{a}A$$.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/vLlauA8EubA" title="Clase59" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/sVytUhMlASs" title="Clase60" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>