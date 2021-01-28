---
layout: distill
title: Quantum typicality methods
description: In quantum statistics, a thermal state in the canonical ensemble is represented by a Gibbs density matrix of the form $\rho = \textrm{e}^{-\beta H}$. Several modern approaches replace the density matrix with a classical ensemble of pure quantum states, called thermal typical states. These reformulations turn out to be extremely useful for numerical simulations. I have employed variants of this technique to investigate several interesting problems, including the stripe and pseudogap physics of the Hubbard model and the thermodynamics of the Shastry-Sutherland model and SrCuBo, which I describe in more detail here.
descriptionfront: In quantum statistics, a thermal state in the canonical ensemble is represented by a Gibbs density matrix of the form \(\rho = \textrm{e}^{-\beta H}\). Several modern approaches replace the density matrix by a classical ensemble of pure quantum states, called thermal typical states. These reformulations turn out to be extremely useful for numerical simulations. I have employed variants of this technique to investigate several interesting problems, including the stripe and pseudogap physics of the Hubbard model and the thermodynamics of the Shastry-Sutherland model and SrCu<sub>2</sub>(BO<sub>3</sub>)<sub>2</sub>, which I describe in more detail here. 
img: /assets/img/shasu.png
importance: 3

bibliography: papers-extended.bib

---

The material SrCu<sub>2</sub>(BO<sub>3</sub>)<sub>2</sub> has been found as one of the first
candidates for realizing a quantum spin
liquid<d-cite key="Smith1991"></d-cite>. Several remarkable observations have been
made in this material, including a pressure-induced quantum phase
transition<d-cite key="Zayed2017"></d-cite> and a fascinating series of
magnetization plateaux<d-cite key="Kageyama1999"></d-cite>. SrCu<sub>2</sub>(BO<sub>3</sub>)<sub>2</sub> is
closely modeled by the so-called Shastry-Sutherland model of
interacting spin-$1/2$ moments. While this model is paradigmatic in
the field of frustrated magnetism, numerical methods have so far not
been capable of simulating finite-temperature properties that could be
compared to actual experimental data. In a recent paper, I have
finally succeeded in simulating the thermodynamic properties of this
model and validating it against experimental specific heat and
susceptibility measurements<d-cite key="Wietek2019"></d-cite>. We find remarkable
agreement between experiment and theory and give a detailed
explanation of the peculiar behavior of these measurements.
This achievement has been made possible by
advancing two numerical techniques, showing convergence in their
respective control parameters while arriving at consistent results.

<div class="row">
    <div class="col-sm-2 mt-3 mt-md-0">
</div>
    <div class="col-sm mt-3 mt-md-1">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/shasu.png' | relative_url }}" alt="" title="example image"/>
	</div>

<div class="col-sm-2 mt-3 mt-md-2">
</div>
</div>
<div class="caption">
   Specific heat measurements of SrCu<sub>2</sub>(BO<sub>3</sub>)<sub>2</sub> agree with
      our numerical predictions from the Shastry-Sutherland model
      <d-cite key="Wietek2019"></d-cite>.
</div>

The technique I developed leading to successful simulations of
SrCu<sub>2</sub>(BO<sub>3</sub>)<sub>2</sub> is based on the concept of thermal typical states.
As a key contribution, I proposed an efficient way of combining this
technique with the Lanczos approximation<d-cite key="Wietek2019"></d-cite>. I have
since applied this technique also to other problems, including a
recent study concerning the physics of high-temperature
superconductors<d-cite key="2012.06589"></d-cite>. While the cuprate
superconductors have important technological applications, the
mechanisms leading to this puzzling phenomenon remain not fully
understood. While the Hubbard model<d-cite key="Zhang1988,Lee2006"></d-cite> of
interacting electrons is believed to capture the most essential
ingredients, our capabilities of simulating this model are still
limited.

Here, I recently demonstrated a clear way forward by developing the
so-called minimally entangled thermal typical state (METTS)
method<d-cite key="White2009,Stoudenmire2010"></d-cite>. The METTS method combines
the strengths of thermal typical states with modern tensor network
algorithms to simulate systems at finite temperature. Even though
tensor network methods have closed in on understanding the ground
state physics<d-cite key="Zheng2017,LeBlanc2015"></d-cite>, finite-temperature
extensions have not yet been successfully applied. This is what I have
now achieved in recent work<d-cite key="Wietek2020"></d-cite>. My simulations
give access to the entire temperature range from the high-temperature
incoherent regime down to essentially ground state temperatures on
cylindrical geometries up to sizes of $32 \times 4$. Focusing on a
particular hole-doping, I establish the onset temperature of the
ground state stripe phase, and discover a novel metallic phase above at
higher temperatures strongly
reminiscent of the pseudogap regime in cuprates.