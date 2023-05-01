---
layout: page
title: Gavillas
description: >
  Definición del concepto de topos
hide_description: true
sitemap: false
---

En esta sección haremos veremos una nueva forma de pensar qué es una topología. En este sentido tenemos el concepto 
clásico con abiertos de un espacio. Luego, Grothendieck observa la importancia de las cubiertas y escribe una versión de 
topología enfatizando esta idea. En esta versión de Lawvere y Tierney se hacen dos cosas al mismo tiempo, una de ellas es 
cambiar la pregunta que hay que responder, de "¿qué cubiertas cubren a un objeto?" a 
"¿a qué objetos cubre una 'cubierta'?". Además de esto también se extiende un poco la lógica interna al dar este concepto 
de topología de tal forma que también resulta ser un operador modal.

### Definición
Una flecha $$j\colon\Omega\to\Omega$$ es una topología de Lawvere-Tierney si satisface $$jv=v$$, $$jj=j$$ y 
$$j(\land)=j\land j$$.

Un ejemplo, que en el futuro será importante, de topología de Lawvere-Tierney es la doble negación 
$$\neg\neg\colon\Omega\to\Omega$$.

Dado un objeto $$E\in\mathcal{E}$$, el concepto de topología permite definir un morfismo 
$$\overline{(-)}\colon Sub(E)\to Sub(E)$$ definiendo $$\overline{A}$$ como el subobjeto de $$E$$ cuya característica es 
$$j\varphi_A$$, donde $$\varphi_A$$ es la característica de $$A\in Sub(E)$$.

En realidad el morfismo de arriba se puede definir con cualquier flecha $$j\colon\Omega\to\Omega$$, pero si la flecha 
$$j$$ es una topología de Lawvere-Tierney, entonces podremos demostrar

$$
A\subseteq\overline{A}\quad
\overline{\overline{A}}=\overline{A}\quad
\overline{A\cap B}=\overline{A}\cap\overline{B}
$$

Una operación en $$Sub(E)$$ que satisfaga las tres igualdades de arriba se llamará *operador de cerradura*. Es importante 
notar que este operador difiere de la cerradura clásica en espacios topológicos donde se cumple 
$$\overline{A\cup B}=\overline{A}\cup\overline{B}$$ en lugar de nuestra tercera igualdad.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/AqXyeV9FHxI" title="Clase50" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

Con la cerradura podemos definir cuando un subobjeto $$A\in Sub(E)$$ es cerrado de manera usual, es decir, si 
$$\overline{A}=A$$ y cuando es denso, $$\overline{A}=E$$. En el segundo caso también diremos que el mono 
$$m\colon A\to E$$ es denso. Con esto damos el concepto de *gavilla*.

### Definición
Un objeto $$F\in\mathcal{E}$$ es una gavilla si para cualquier mono denso $$m\colon A\to E$$ y toda flecha 
$$f\colon A\to F$$ existe una única $$g\colon E\to F$$ tal que $$gm=f$$.

Otra forma de decir que un objeto $$F$$ es una gavilla es mediante la función "componer con $$m$$". Esto es, $$F$$ es 
gavilla si y sólo si la función

$$
m^*\colon \mathcal{E}(E,F)\to\mathcal{E}(A,F)
$$

es biyectiva para todo mono denso $$m\colon A\to E$$.

Además de las gavillas otros objetos de interés son aquellos para los cuales la función de arriba es inyectiva. Cuando un 
objeto satisfaga esto diremos que es un objeto *separado*. Con estos dos tipos de objetos formamos dos subcategorías 
plenas del topos $$\mathcal{E}$$, la de objetos gavilla, denotada $$Gav_j(\mathcal{E})$$, y la de objetos separados, 
denotada $$Sep_j(\mathcal{E})$$.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/1wVTr15DyrE" title="Clase51" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

Las dos subcategorías $$Gav_j(\mathcal{E})$$ y $$Sep_j(\mathcal{E})$$ tienen buenas propiedades. Por ejemplo, ambas tienen límites finitos y son cerradas bajo exponenciales.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/R13KOym5010" title="Clase52" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>