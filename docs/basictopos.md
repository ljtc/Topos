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

<iframe width="560" height="315" src="https://www.youtube.com/embed/h7j0MYBp6Fg" title="Clase17" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


## Construcción de exponenciales
En la definición de topos (elemental) ne se pidió que fuera una categoría cartesiana cerrada, ni siquiera que existan 
objetos exponencial. En el tercer axioma se pide la existencia de objetos potencia. Estos objetos son, como en conjuntos, 
lo mismo que exponenciar con base el clasificador de subobjetos. çse puede demostrar que esto es todo lo que se necesita 
para obtener una categoría cartesiana cerrada (por supuesto, no sólo se usará el tercer axioma en la demostración).

Podemos pensar que la construcción está hecha en dos partes. En la primera necesitamos construir un objeto $$C^B$$ para 
cualesquiera $$B,C\in\mathcal{E}$$. Esta construcción se basa fuertemente en lo que sucede en conjuntos, específicamente 
cuando un subconjunto $$S\subseteq C\times B$$ es la gráfica de una función $$f\colon B\to C$$.

<iframe width="560" height="315" src="https://www.youtube.com/embed/GBVeeYTWUcA" title="Clase18" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

En la segunda parte de la construcción de exponenciales se demuestra que un topos es una categoría cartesiana cerrada. 
Esto es, se muestra la existencia de la flecha evaluación $$ev_{B,C}\colon B\times C^B$$ y se muestra que es una flecha 
universal de $$B\times -$$ a C. Esta flecha evaluación se volverá la counidad de la adjunción

$$
(B\times -) \; \dashv\; ()^B
$$

terminando la demostración de que un topos es una categoría cartesiana cerrada.

Una vez que ya hemos hecho todo la anterior tenemos aún más ya que $$C^B$$ se puede interpretar como un $$hom$$ interno, 
en el sentido que $$\mathcal{E}(B,C)\sim C^B$$. Además, también es posible definir la composición como una operación 
interna, es decir, hay una flecha $$m\colon B^A\times C^B\to C^A$$ que satisface: si $$f\colon A\to B$$ y 
$$g\colon B\to C$$, entonces $$m(\hat{f},\hat{g})=\hat{gf}$$.

<iframe width="560" height="315" src="https://www.youtube.com/embed/cQo96rclkyI" title="Clase19" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


## Imagen directa
Empezaremos haciendo una simplificación del problema. En lugar de tomar una flecha arbitraria para calcular imágenes 
directas tomaremos un mono. Sea $$m\colon B'\rightarrowtail B$$ un mono en $$\mathcal{E}$$. Es posible construir una 
flecha $$\exists_k\colon PB'\to PB$$ que "calcule" la imagen directa de un subobjeto de $B'$ respecto a la flecha $$k$$.
En otras palabras, se construye $$\exists_k$$ y se demuestra que si $$m\colon S\rightarrowtail B'$$ es mono entonces

$$
\exists_k\, \hat{\varphi_m}\;=\;\hat{\varphi_{mk}}
$$

Una propiedad importante de la imagen directa es una relación con el funtor potencia.

### Teorema (Beck-Chevalley)
