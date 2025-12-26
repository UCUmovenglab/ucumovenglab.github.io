---
title: Contacto
nav_title: Contacto
lang: es
ref: contact
nav:
  order: 3
  tooltip: Cómo contactarnos
---

# {% include icon.html icon="fa-regular fa-envelope" %}Contacto

¡Nos encantaría saber de usted!

{%
  include button.html
  type="email"
  text="pablo.iturralde@ucu.edu.uy"
  link="pablo.iturralde@ucu.edu.uy"
%}
{%
  include button.html
  type="email"
  text="enrique.ferreira@ucu.edu.uy"
  link="enrique.ferreira@ucu.edu.uy"
%}

{% include section.html %}

## Ubicación

Universidad Católica del Uruguay
Facultad de Ingeniería y Tecnologías
Av. 8 de Octubre 2738
Montevideo, Uruguay

{% include section.html %}

## Nuestro Equipo

{% include list.html data="members" component="portrait" filters="role: pi" %}
