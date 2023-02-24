---
layout: page
title: Teorema de Beck
description: >
  Terminamos nuestro repaso de categorías con el teorema de Beck
hide_description: true
sitemap: false
---

En la [sección de mónadas](https://ljtc.github.io/topos/docs/monadas.md) vimos, dada una adjunción, la existencia de un funtor de comparación $$K\colon\mathbf{B}\to\mathbf{A}^T$$. Ahora daremos condiciones suficientes para que este funtor sea una equivalencia de categorías. Cuando esto suceda diremos que el funtor $$G\colon\mathbf{B}\to\mathbf{A}$$ es *monádico*.

### Teorema (Beck)
Sea $$G\colon\mathbf{B}\to\mathbf{A}$$ un funtor con adjunto izquierdo $$F\colon\mathbf{A}\to\mathbf{B}$$. Sean 
$$(T,\eta,\mu)$$ la mónada inducida y $$\mathbf{A}^T$$ la categoría de $$T$$-álgebras.
1. Si $$\mathbf{B}$$ tiene coigualadores de pares reflexivos, entonces el funtor de comparación $$K$$ tiene adjunto izquierdo $$L$$.
2. Supongamos qu,e además de lo anterior, $$G$$ preserva coigualadores, entonces la unidad de la adjunción $$L\dashv K$$ es un isomorfismo.
3. Si además $$G$$ refleja isomorfismos, entonces la counidad de $$L\dashv K$$ es un isomorfismo.
