---
layout: default
title: About
---

<p class="lead">
I'm a 2026 graduate in Civil and Environmental Engineering from the Islamic University of
Technology (IUT), Dhaka, working in geotechnical engineering. My thesis asked whether the
settlement above a shallow tunnel can be predicted <em>before</em> the tunnel is built —
from how the tunnel wall moves, rather than by fitting a curve to measurements after the
fact.
</p>

Empirical practice reduces a settlement trough to a single ground loss ratio, which
assumes the ground only cares how much soil is lost, not how the tunnel cross-section
deforms. Model tests say otherwise: two excavation patterns at identical ground loss
produce visibly different troughs. I tested an analytical unified displacement function
and a physics-informed neural network against experiments where the tunnel-wall movement
was imposed and known — so the prediction is genuinely out-of-sample rather than
back-fitted. The elastic solution gets the depth of the trough right to within 12%, but
spreads it about twice too wide; a two-parameter width correction raises the mean R²
from 0.41 to 0.91.

Alongside the thesis I work on numerical foundation modelling in PLAXIS 3D — my Final
Year Design Project took pile and raft systems for a multi-storeyed building to failure
to extract bearing capacity and settlement. In October 2025 I trained at DOHWA
Engineering in Dhaka, on the consultancy side of geotechnical work.

### Research interests

- **Tunnelling-induced ground movement** — how the shape of tunnel-wall deformation, not
  just the volume lost, controls the surface settlement trough.
- **Physics-informed machine learning in geomechanics** — where a PINN genuinely adds
  something over a closed-form elastic solution, and where it just reproduces it slower.
- **Numerical modelling of foundations** — pile and raft behaviour in PLAXIS, and how far
  design-stage models track observed capacity.

### News

<ul class="news">
{% for item in site.data.news %}
  <li>
    <span class="date">{{ item.date }}</span>
    <span>{{ item.text | markdownify | remove: '<p>' | remove: '</p>' | strip }}</span>
  </li>
{% endfor %}
</ul>

<div class="callout" markdown="1">
**Contact.** Email me at [{{ site.author.email }}](mailto:{{ site.author.email }}).
Happy to share the analysis code or the full thesis on request.
</div>
