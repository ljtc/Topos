---
layout: page
title: Límites
description: >
  Los límites serán la principal forma de construir objetos en nuestras categorías
hide_description: true
sitemap: false
---

# Límites
Las categorías que estaremos estudiado, *topos elementales*, deben tener un gran poder constructivo ya que podrán ser 
usadas como fundamentos locales de las matemáticas. Las construcciones categóricas se hacen por medio de propiedades 
universales y los límites serán objetos "de cierta forma" que satisfacen una propiedad universal. Así que nos será útil tener algunos resultados básicos acerca de estos objetos.

## Conos
Si estudiamos el comportamiento de límites conocidos en algunas categorías, como el producto cartesiano y la imagen inversa en conjuntos o el kernel en módulos, entonces podemos notar que estas construcciones empiezan escogiendo objetos y flechas en alguna categoría y luego encontrando un objeto especial para lo que escogimos.

Para escoger objetos y flechas en una categoría $$\mathbf{C}$$ podemos considerar un funtor que salga de una "categoría de índices". Así, un funtor $$\Gamma\colon\mathbf{I}\to\mathbf{C}$$ es llamado 
*diagrama de forma $$\mathbf{I}$$ en $$\mathbf{C}$$*.

Luego, dado un diagrama $$\Gamma\colon\mathbf{I}\to\mathbf{C}$$ un cono es un objeto $$L\in\mathbf{C}$$ junto con flechas
$$(L\xrightarrow{\pi_I}\Gamma I)_{I\in\mathbf{I}}$$ tal que para cualquier flecha $$i\colon I\to J$$ en $$\mathbf{I}$$
se tiene que $$\Gamma i\pi_I =\pi_J$$. El objeto $$L$$ se llama *vértice del cono*.

## Límites
Un diagrama puede tener muchos vértices así que no son suficientes para definir un objeto. Para lograr la unicidad (salvo isomorfismo) pediremos una propiedad universal: para cualquier otro cono 
$$(A\xrightarrow{\alpha_I}\Gamma I)_{I\in\mathbf{I}}$$ existe una única $$h\colon A\to L$$ tal que $$\pi_I h=\alpha_I$$.


<iframe width="560" height="315" src="https://www.youtube.com/embed/1Vc842ZqgeM" title="Clase7" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>