---
layout: page
title: Mónadas
description: >
  Exploraremos una relación entre adjunciones y ciertos conceptos algebraicos
hide_description: true
sitemap: false
---

## Definición
Una *mónada* es una terna $$(T,\eta,\mu)$$ donde $$T\colon\mathbf{A}\to\mathbf{A}$$ es un funtor, 
$$\eta\colon Id_{\mathbf{A}}\to GF$$ y $$\mu\colon FG\to Id_{\mathbf{A}}$$ son transformaciones naturales. $$\eta$$ es la *unidad* y $$\mu$$ es la multiplicación de la mónada. Estas transformaciones deben satisfacer la versión diagramática de que $$\mu$$ es asociativa y $$\eta$$ es neutro para $$\mu$$.

El tema de mónadas es bastante extenso y profundo, además de tener aplicaciones a otras áreas, como computación. Sin embargo, aquí sólo veremos que toda adjunción induce una mónada y viceversa, toda mónada induce una adjunción

