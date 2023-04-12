---
layout: page
title: Construcción de colímites
description: >
  Definición del concepto de topos
hide_description: true
sitemap: false
---


Ahora usaremos al funtor potencia para mostrar que un topos elemental tiene todos los colímites finitos. Para lograr esto 
usaremos la versión del [teorema de Beck](./beck.md) que mostramos antes para mostrar que el funtor potencia es monádico. 
Gracias a Beck-Chevalley ya tenemos que potencia preserva coigualadores de pares reflexivos en $$\mathcal{E}^{op}$$ (es 
decir, de pares correflexivos en $$\mathcal{E}$$).

Siguiendo con la demostración de que el funtor potencia es monádico, no es difícil mostrar que es adjunto izquierdo de 
$$P\colon\mathcal{E}^{op}\to\mathcal{E}$$ es $$P^{op}\colon\mathcal{E}\to\mathcal{E}^{op}$$. En este caso lo más fácil es mostrar que hay una biyección natural

$$
\mathcal{E}^{op}(P^{op}A,B) \cong \mathcal{E}(A,PB)
$$

De la biyección podemos extraer las componentes de la unidad $$\eta_A\colon A\to PPA$$, que en conjuntos es la función que 
a cada $$a\in A$$ la manda a $$\{S\subseteq A\mid a\in S\}$$, y las componentes de la counidad 
$$\varepsilon_B\colon PPB\to B$$, que en este caso es simplemente $$(\eta_B)^{op}$$. Además las dos identidades triangulares se reducen a 

$$
P\eta_A\, \eta_{PA}=id_{PA}
$$

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/8Eb5fscm_m4" title="Clase23" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

Como $$\mathcal{E}$$ tiene todos los límites finitos, entonces $$\mathcal{E}^{op}$$ tiene coigualadores de pares 
reflexivos. Así, sólo falta mostrar que $$P$$ refleja isomorfismos. La demostración consta de varios pasos. Primero se 
muestra que el funtor $$P$$ es fiel. Luego se demuestra que cualquier funtor fiel preserva monomorfismos y epimorfismos. 
También hay que notar que en un topos una flecha que es monomorfismo y epimorfismo es un isomorfismo. Finalmente, se 
"pegan" estos resultados para obtener lo que queremos.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/iNhF7BoXkSA" title="Clase24" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

Una vez que ya sabemos que $$P\colon\mathcal{E}^{op}\to\mathcal{E}$$ es monádico, obtenemos una equivalencia
$$(L,K,\alpha,\beta)\colon\mathcal{E}^T\to\mathcal{E}^{op}$$. Esta equivalencia nos da un camino para mostrar la 
existencia de colímites en el topos $$\mathcal{E}$$. Para poder seguir dicho camino, se demuestra que el funtor que olvida 
$$G^T\colon\mathcal{E}^{T}\to\mathcal{E}$$ crea límites y que si $$L\dashv K$$ es una equivalencia, entonces $$L$$ 
preserva límites.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/agQcOPsgyQ0" title="Clase25" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

Ahora ya podemos demostrar que un topos tiene colímites finitos. Si tomamos un diagrama 
$$\Gamma\colon\mathbf{I}\to\mathcal{E}$$ con $$\mathbf{I}$$ finita, entonces demostrar que $$\Gamma$$ tiene colímite (en 
$$\mathcal{E}$$) es lo mismo que demostrar que $$\Gamma^{op}$$ tiene límite (en $$\mathcal{E}^{op}$$). Este límite se 
obtiene del diagrama $$K\Gamma^{op}\colon\mathbf{I}^{op}\to\mathcal{E}^{T}$$ y el hecho de que $$G^T$$ crea límites.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/JcyAzHyJXig" title="Clase26" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>