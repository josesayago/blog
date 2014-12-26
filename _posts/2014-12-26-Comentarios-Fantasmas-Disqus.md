---
layout: post
title:  "Comentarios Fantasmas en Disqus"
date:   2014-12-26 00:55:00
categories: bugs
---

Hace un tiempo decidí cambiar la estructura de enlaces permanentes de mis blogs en <a href="http://8elite.com" title="8ª Elite">8ª Elite</a>, esto trajo como consecuencia que los comentarios a través de Disqus desaparecieran. Revisando el panel de control de mis cuentas éstos aún eran visibles, pero no cuando accedía a los artículos a través de mi sitio.

Resulta que debido al cambio de estructura de enlaces permanentes, Disqus no podía enlazar el hilo de comentarios a los artículos puesto que la dirección para enlazarlos estaba rota.

Disqus pone a disposición tres <a href="https://help.disqus.com/customer/portal/articles/286778-migration-tools">herramientas de migración</a> que permiten fácilmente solucionar este problema. En mi caso ya que cada URL migrada a la nueva estructura contaba con una redirección 301, utilicé <em>Redirect Crawler</em> que detecta automáticamente las nuevas URL usando las redirecciones presentes en las antiguas URL.