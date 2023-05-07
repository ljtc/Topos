---
layout: page
title: Funtor gavilla asociada
description: >
  Definición del concepto de topos
hide_description: true
sitemap: false
---

En esta sección veremos que la inclusión $$\mathcal{E}_j\to\mathcal{E}$$ tiene un adjunto izquierdo que preserva límites 
finitos. La demostración se hará en dos pasos, primero veremos que la inclusión $$Sep_j\mathcal{E}\to\mathcal{E}$$ tiene 
adjunto izquierdo y luego veremos lo correspondiente con la inclusión $$\mathcal{E}_j\to Sep_j\mathcal{E}$$.

Como los objetos separados tienen un papel central en esta sección, empezamos viendo algunas equivalencias de ser 
separado. Más específicamente, los siguientes enunciados son equivalentes:
1. $$C$$ es separado;
2. la diagonal, $$\Delta_C\colon C\to C\times C$$ es cerrada;
3. $$j^C \{\,\}_C=\{\,\}_C$$;
4. Para cualquier flecha $$f\colon A\to C$$, la gráfica de $$f$$ es un subobjeto cerrado de $$A\times C$$.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/0PFNr0_S41A" title="Clase55" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>

Ahora empezamos a construir un funtor $$\mathcal{E}\to Sep_j\mathcal{E}$$. Para cada $$E\in\mathcal{E}$$ consideramos la 
composición $$r^E \{\,\}_E$$ y su factorización epi-mono. Si $$\theta_E\colon E\to E'$$ es el epi de la factorización 
anterior, entonces podemos demostrar que $$E'$$ es un objeto separado. Con esto podemos definir la asignación en objetos 
del funtor anterior, $$E\mapsto E'$$. Para demostrar que $$E'$$ es separado se observa que $$\Omega_{j}^{E}$$ es una 
gavilla inyectiva y como tenemos un mono $$E'\rightarrowtail \Omega_{j}^{E}$$ de la factorización epi-mono, entonces 
$$E'$$ es separado, como queríamos.

Una propiedad más acerca de la construcción del epi $$\theta_E\colon E\to E'$$ del párrafo anterior es que si $$E$$ es separado, entonces $$\theta_E$$ es iso. Así, concluimos que $$E$$ es separado si y sólo si $$E$$ se puede encajar en una gavilla inyectiva $$E\rightarrowtail I_E$$.

Finalmente, veremos que el par núcleo del epi $$\theta_E\colon E\to E'$$ es la cerradura de la diagonal.

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/uaVmzuq4-OY" title="Clase56" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>