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
<iframe width="560" height="315" src="https://www.youtube.com/embed/9UMYx25AtMM" title="Clase 31" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

Ahora sólo falta ver que $$\mathcal{E}/B$$ tiene objetos potencia. Lo primero que haremos para demostrar este hecho es notar que el axioma de objetos potencia es equivalente a que haya una biyección

$$\mathcal{E}(A\times C,\Omega)\cong\mathcal{E}(C,PA)$$

natural en $$A$$ y $$C$$. Así, para cada $$f\colon C\to B$$ en $$\mathcal{E}/B$$ encontraremos un objeto, que denotaremos $$P_B f$$ tal que para cualquier $$g\colon D\to B$$ haya una biyección

$$\mathcal{E}/B(C\times_B D,\Omega\times B)\cong\mathcal{E}/B(D,P_B f)$$

natural en $$C$$ y $$D$$.

Empezamos analizando el lado izquierdo de la biyección que queremos, para esto primero daremos una forma conveniente de la 
característica de $$C\times_B D$$ como subobjeto de $$C\times D$$. Además, notamos que una flecha 
$$C\times_B D\to\Omega\times B$$ en $$\mathcal{E}/B$$ está en correspondencia con una flecha $$C\times_B D\to\Omega$$ en 
$$\mathcal{E}$$ y esta con un subobjeto de $$C\times_B D$$, que a su vez es lo mismo que un subobjeto de $$C\times D$$ 
contenido en $$C\times_B D$$.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/TX2auzwmxC4" title="Clase 32" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
<iframe width="560" height="315" src="https://www.youtube.com/embed/7UT_pz8Tqaw" title="Clase 33" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

La siguiente biyección natural se sigue de notar que todo subobjeto tiene una flecha característica. De esta forma, si 
empezamos con un un subobjeto $$S$$ de $$C\times D$$ contenido en $$C\times_B D$$ y recordamos que la característica de 
$$C\times_B D$$ es $$\in_C(id\times w)$$, entonces la característica de $$S$$ satisface:

$$\varphi_S\land \in_C(id,w)=\varphi_S$$

donde $$\land$$ es la flecha $$\land\colon\Omega\times\Omega\to\Omega$$.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/y27Jp9q59bY" title="Clase 34" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

La siguiente biyección natural es consecuencia de tomar $$P$$-transpuestas. Además, también hay que notar que si la característica de $$S$$ satisface la ecuación de arriba, entonces su $$P$$-transpuesta satisface:

$$\hat{\varphi}_S\land w=\hat{\varphi}_S$$

donde $$\land$$ es la flecha $$\land\colon PC\times PC\to PC$$.

La última biyección consiste en reescribir la ecuación anterior para obtener un par de flechas 
$$p_1,t\colon PC\times B\to PC$$ de tal forma que si $$\hat{\varphi}_S$$ satisface la ecuación de arriba, entonces 
$$(\hat{\varphi}_S,g)$$ iguala al par $$(p_1,t)$$. 

Definimos el objeto potencia del objeto $$f\colon C\to B$$ en $$\mathcal{E}/B$$ como el igualador del par $$(p_1,t)$$ seguido de la proyección al segundo factor

$$P_B f\xrightarrow{e}PC\times B\xrightarrow{p_2}B$$

Con lo anterior podemos concluir que si $$\hat{\varphi}_S$$ satisface la ecuación de arriba, entonces hay una única flecha 
$$h:D\to P_B f$$ tal que $$eh=(p_1,t)$$ dada por la propiedad universal del igualador.

Así, podemos concluir que hay una biyección natural

$$\mathcal{E}/B(C\times_B D,\Omega\times B)\cong\mathcal{E}/B(D,P_B f)$$

como queríamos.

<p>
<iframe width="966" height="543" src="https://www.youtube.com/embed/1_AqoSEKnSk" title="Clase 35" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

---

Ahora, dada una flecha $$k\colon B\to A$$ podemos definir un funtor, llamado *cambio de base*,
$$k^*\colon\mathcal{E}/A\to\mathcal{E}/B$$ que actúa por medio de producto fibrado a lo largo de $$k$$. Lo primero que veremos del funtor cambio de base es:

### Teorema
$$k^*\colon\mathcal{E}/A\to\mathcal{E}/B$$ tiene adjuntos derecho e izquierdo.

La demostración del teorema se hace en dos pasos, primero se analiza la situación $$A=1$$, de tal forma que $$k$$ es la única flecha al terminal.

<p>
<iframe width="1440" height="679" src="https://www.youtube.com/embed/Bionrwt582s" title="Clase 36" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

El siguiente paso es tomar $$k\colon B\to A$$ arbitraria y notar que $$\mathcal{E}/B\cong(\mathcal{E}/A)/k$$. Así, podemos aplicar el caso anterior para obtener el resultado del teorema.

<p>
<iframe width="1440" height="679" src="https://www.youtube.com/embed/L14PgRmUCP4" title="Clase 37" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

Se puede demostrar aún más del funtor cambio de base. Este funtor es un *morfismo lógico*, es decir, preserva límites finitos, clasificador de subobjetos y exponenciales (todo salvo iso). 

### Teorema
$$k^*\colon\mathcal{E}/A\to\mathcal{E}/B$$ es un morfismo lógico.

La preservación de límites se sigue de que tiene adjunto izquierdo y es fácil ver que preserva al clasificador de subobjetos. Así, la parte interesante de la demostración es que preserva exponenciales.

Usando los dos teoremas anteriores es posible demostrar algunas cosas similares a lo que pasa en la categoría de conjuntos.

<p>
<iframe width="1440" height="679" src="https://www.youtube.com/embed/A_BK-QHPB8w" title="Clase 38" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>