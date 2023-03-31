---
layout: page
title: Definición de topos
description: >
  Definición del concepto de topos
hide_description: true
sitemap: false
---

### Definición
Una categoría $$\mathcal{E}$$ es un topos elemental si satisface
1. $$\mathcal{E}$$ tiene límites finitos,
2. $$\mathcal{E}$$ tiene clasificador de subobjetos $$\Omega$$,
3. $$\mathcal{E}$$ tiene objetos potencia.

Un clasificador de subobjetos es un objeto $$\Omega$$ junto con una flecha $$v\colon 1\to\Omega$$ tal que para cualquier 
mono $$m\colon S\to A$$ existe una única *flecha característica* $$\varphi_m\colon A\to\Omega$$ tal que el cuadrado 
conmutativo generado por $$v\,!_S=\varphi_m\,m$$ es un producto fibrado.

Dado un objeto $$A\in\mathcal{E}$$ el *objeto potencia* de $$A$$ es un objeto $$PA$$ junto con una flecha 
$$\in_A\colon A\times PA\to\Omega$$ universal, es decir, para cada $$f\colon A\times B\to\Omega$$ existe una única 
$$\hat{f}\colon B\to PA$$ tal que $$\in_A(\text{id}\times\hat{f})=f$$. La flecha $$\hat{f}$$ será llamada la 
$$P$$-transpuesta de $$f$$.

Regresando al clasificador de subobjetos, notamos que define una biyección

$$
  \mathcal{E}(A,\Omega)\cong Sub_{\mathcal{E}}(A).
$$

Esta biyección es muy importante para tener una forma de hablar de la colecciones de sunobjetos sin hacer referencia a la teoría de conjuntos.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/ieSLALPW57c" title="Clase16" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

Ahora tomemos en cuenta a los objetos potencia y al clasificador de subobjetos, además del isomorfismo 
$$A\times 1\cong A$$. Dado un subobjeto $$m\colon S\to A$$, consideramos su flecha característica 
$$\varphi_m\colon A\to\Omega$$ y con el iso anterior se tiene la composición 
$$A\times 1\to A\xrightarrow{\varphi_m}\Omega$$. Así, hay una única $$\hat{\varphi_m}\colon 1\to\Omega$$ que hace conmutar al diagrama de la definición de objetos potencia.

Con lo anterior tenemos tres formas de pensar un subobjeto de $$A$$: como un mono
$$m\colon S\to A$$, como una flecha característica $$\varphi_m\colon A\to\Omega$$ o como un elemento global
$$\hat{\varphi_m}\colon 1\to PA$$

Se puede demostrar que si $$m\colon S\to A$$ es mono entonces la única 
$$\varphi_m\colon A\to\Omega$$ es de hecho una flecha característica. Para mostrar esto denotamos con $$v_X$$ a la 
composición $$X\xrightarrow{!_X}1\xrightarrow{v}\Omega$$ y notemos que 
$$\varphi_m\,x=v_X \iff \in_A(x,\hat{\varphi_m})=v_X$$.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/fttIatTFWFE" title="Clase17" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

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


