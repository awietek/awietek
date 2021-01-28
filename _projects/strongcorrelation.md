---
layout: distill
title: Strongly correlated electrons
description: To answer why matter behaves the way it does we need to understand how macroscopic physics emerges from the microscopic laws describing the motions of electrons and atoms. Naturally, things become interesting if particles interact strongly and their collective behavior is starkly different from the behavior of individual constituents. The strange laws of quantum mechanics describing electrons and atoms add some additional spice, but also complexity to this endeavor. I am studying fundamental models describing the physics of interacting electrons to understand how different states of matter emerge. This includes the stripe and pseudogap physics of the hole-doped Hubbard model at finite-temperature which I studied using a tensor network technique called METTS. 
img: /assets/img/snapshots.png
importance: 1

bibliography: papers-extended.bib

---
<p>
  Superconductivity, charge density waves and antiferromagnetism are
  prominent features of cuprate high-temperature superconductors. The
  basic mechanisms of these materials are believed to be described by
  one of the most fundamental models in solid-state physics, the
  Hubbard model. While several analytical and numerical techniques
  approach the problem from the high-temperature limit, tensor network
  methods, like the density matrix renormalization group (DMRG) have
  been used to study ground state properties of the system. Even
  though tensor network methods alongside other approaches have closed
  in on an understanding of the ground state
  physics<d-cite key="Zheng2017,Huang2018,LeBlanc2015"></d-cite>,
  finite-temperature extensions of tensor network methods have not yet
  been successfully applied to the Hubbard model.  This is what I have
  now achieved in a recent work<d-cite key="Wietek2020"></d-cite>.
  By combining recent
  developments in tensor network approaches for imaginary time
  evolution with high-accuracy Krylov methods I demonstrated that
  controlled and accurate simulations of the strongly interacting
  Hubbard model at finite temperature and finite doping can be
  successfully performed. Our simulations using the so-called METTS
  method<d-cite key="White2009"></d-cite>, give us access to study the entire
  temperature range from the high-temperature incoherent regime down
  to essentially ground state temperatures on cylindrical geometries
  up to sizes of \(32 \times 4\).  Focusing on a particular hole-doping,
  we establish the onset temperature of the ground state stripe phase
  as shown in the figure below and discover a novel metallic phase
  above at higher temperatures strongly reminiscent of the pseudogap
  regime in cuprates.

</p>


<div class="row">
    <div class="col-sm mt-1 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/snapshotsbig.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
   Illustration stripe order at hole-doping \(p=1/16\) in the
      Hubbard model of high-temperature superconductors at interaction
      strength \(U/t=10\) and temperature
      \(T/t=0.025\)<d-cite key="Wietek2020"></d-cite>.
</div>