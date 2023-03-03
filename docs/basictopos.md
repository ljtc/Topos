---
layout: page
title: Construcciones básicas
description: >
  Ahora veremos cómo se hacen algunas construcciones con sólo los tres axiomas de topos.
hide_description: true
sitemap: false
---

## Construcción de exponenciales
En la definición de topos (elemental) ne se pidió que fuera una categoría cartesiana cerrada, ni siquiera que existan 
objetos exponencial. En el tercer axioma se pide la existencia de objetos potencia. Estos objetos son, como en conjuntos, 
lo mismo que exponenciar con base el clasificador de subobjetos. çse puede demostrar que esto es todo lo que se necesita 
para obtener una categoría cartesiana cerrada (por supuesto, no sólo se usará el tercer axioma en la demostración).

Podemos pensar que la construcción está hecha en dos partes. En la primera necesitamos construir un objeto $$C^B$$ para 
cualesquiera $$B,C\in\mathcal{E}$$. Esta construcción se basa fuertemente en lo que sucede en conjuntos, específicamente 
cuando un subconjunto $$S\subseteq C\times B$$ es la gráfica de una función $$f\colon B\to C$$.

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


## Imagen directa
Empezaremos haciendo una simplificación del problema. En lugar de tomar una flecha arbitraria para calcular imágenes 
directas tomaremos un mono. Sea $$m\colon B'\tailrightarrow B$$ un mono en $$\mathcal{E}$$. Es posible construir una 
flecha $$\exists_k\colon PB'\to PB$$ que "calcule" la imagen directa de un subobjeto de $B'$ respecto a la flecha $$k$$.
En otras palabras, se construye $$\exists_k$$ y se demuestra que si $$m\colon S\tailrightarrow B'$$ es mono entonces

$$
\exists_k\, \hat{\varphi_m}\;=\;\hat{\varphi_{mk}}
$$

Una propiedad importante de la imagen directa es una relación con el funtor potencia.

### Teorema (Beck-Chevalley)
