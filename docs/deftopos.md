---
layout: page
title: Definición de Topos Elemental
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

<p> </p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/ieSLALPW57c" title="Clase16" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

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

<p> </p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/fttIatTFWFE" title="Clase17" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


## Construcción de exponenciales
