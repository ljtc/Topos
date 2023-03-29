---
layout: page
title: Construcciones básicas
description: >
  Ahora veremos cómo se hacen algunas construcciones con sólo los tres axiomas de topos.
hide_description: true
sitemap: false
---

## Algunos predicados
Más adelante veremos que el clasificador de subobjetos creará una lógica interna para el topos. Hará eso de tal forma que 
una flecha $$A\to\Omega$$ será una fórmula con una variable libre de tipo $$A$$. Usaremos esta intuición y llamaremos 
predicados a las flechas que construiremos en esta sección.

Con la propiedad universal del producto es posible construir la flecha *diagonal* $$\Delta_A\colon A\to A\times A$$. Esta 
es la flecha con la propiedad de que al componerla con cualquiera de las dos proyecciones se obtiene la identidad. Es 
fácil ver que la diagonal es un mono y así tiene una flecha característica $$\delta_A\colon A\times A\to Omega$$. Este predicado, o fórmula con dos variables libres de tipo $$A$$, satisface que si tomamos elementos generalizados 
$$x,y\colon X\to A$$ entonces

$$
\delta_A(x,y)=v_X \iff x=y
$$

Así, $$\delta_A$$ es el predicado de igualdad en $$A$$ o la delta de Kronecker.

Ahora, tomamos la $$P$$-transpuesta de $$\delta_A$$ y obtenemos la flecha *unitario* $$\{\cdot\}\colon A\to PA$$. La flecha unitario satisface, para cualesquiera $$x,y\colon X\to A$$,

$$
\in_A(x,\{y\})=v_X \iff x=y
$$

La equivalencia anterior muestra que nuestra flecha unitario de verdad se comporta como un conjunto unitario. Además, como es de esperar, también es mono; por lo que tiene una flecha característica $$\sigma_A\colon PA\to\Omega$$. Si $$x\colon X\to PA$$, entonces $$\sigma_A$$ satisface

$$
\sigma_A(x)=v_X \iff \exists X\xrightarrow{y}A(x=\{y\})
$$

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/h7j0MYBp6Fg" title="Clase17" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>


## Construcción de exponenciales
En la definición de topos (elemental) ne se pidió que fuera una categoría cartesiana cerrada, ni siquiera que existan 
objetos exponencial. En el tercer axioma se pide la existencia de objetos potencia. Estos objetos son, como en conjuntos, 
lo mismo que exponenciar con base el clasificador de subobjetos. çse puede demostrar que esto es todo lo que se necesita 
para obtener una categoría cartesiana cerrada (por supuesto, no sólo se usará el tercer axioma en la demostración).

Podemos pensar que la construcción está hecha en dos partes. En la primera necesitamos construir un objeto $$C^B$$ para 
cualesquiera $$B,C\in\mathcal{E}$$. Esta construcción se basa fuertemente en lo que sucede en conjuntos, específicamente 
cuando un subconjunto $$S\subseteq C\times B$$ es la gráfica de una función $$f\colon B\to C$$.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/GBVeeYTWUcA" title="Clase18" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

En la segunda parte de la construcción de exponenciales se demuestra que un topos es una categoría cartesiana cerrada. 
Esto es, se muestra la existencia de la flecha evaluación $$ev_{B,C}\colon B\times C^B$$ y se muestra que es una flecha 
universal de $$B\times -$$ a C. Esta flecha evaluación se volverá la counidad de la adjunción

$$
(B\times -) \; \dashv\; ()^B
$$

terminando la demostración de que un topos es una categoría cartesiana cerrada.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/cQo96rclkyI" title="Clase19" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

Una vez que ya hemos hecho todo la anterior tenemos aún más ya que $$C^B$$ se puede interpretar como un $$hom$$ interno, 
en el sentido que $$\mathcal{E}(B,C)\sim C^B$$. Además, también es posible definir la composición como una operación 
interna, es decir, hay una flecha $$m\colon B^A\times C^B\to C^A$$ que satisface: si $$f\colon A\to B$$ y 
$$g\colon B\to C$$, entonces $$m(\hat{f},\hat{g})=\hat{gf}$$.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/6RZoANxEgX8" title="Clase20" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>


## Imagen directa
Empezaremos haciendo una simplificación del problema. En lugar de tomar una flecha arbitraria para calcular imágenes 
directas tomaremos un mono. Sea $$m\colon B'\rightarrowtail B$$ un mono en $$\mathcal{E}$$. Es posible construir una 
flecha $$\exists_k\colon PB'\to PB$$ que "calcule" la imagen directa de un subobjeto de $B'$ respecto a la flecha $$k$$.
En otras palabras, se construye $$\exists_k$$ y se demuestra que si $$m\colon S\rightarrowtail B'$$ es mono entonces

$$
\exists_k\, \hat{\varphi_m}\;=\;\hat{\varphi_{mk}}
$$

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/k1dXMRBnrEs" title="Clase21" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

Una propiedad importante de la imagen directa es una relación con el funtor potencia.

### Teorema (Beck-Chevalley)

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/62OaRLZ0asI" title="Clase22" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>


## Construcción de colímites
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


## Factorización e imagen
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

