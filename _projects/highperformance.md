---
layout: distill
title: High Performance Computing for quantum many-body systems
description: The quantum many-body problem is exponentially hard in the number of particles. For quantum spin systems the Hilbert space dimension scales as $2^N$, where $N$ denotes the number of spins. I have been working on high-performance computing aspects of exact diagonalization by developing novel algorithms for employing conservation laws and distributed memory parallelization. The implementation of these ideas led to the first exact ground state simulation of an $N=50$ spin system.
descriptionfront: The quantum many-body problem is exponentially hard in the number of particles. For quantum spin systems the Hilbert space dimension scales as \(2^N\), where \(N\) denotes the number of spins. I have been working on high-performance computing aspects of exact diagonalization by developing novel algorithms for employing conservation laws and distributed memory parallelization. The implementation of these ideas led to the first exact ground state simulation of an \(N=50\) spin system.
img: /assets/img/speedup.png
importance: 4
bibliography: papers-extended.bib
---
<p>
  Exact diagonalization is a fundamental and versatile technique to study
  quantum many-body systems. Since it does not perform any approximations,
  it can yield reliable insights if the calculations can be performed on a
  system large enough to capture the essential physical phenomena. However,
  due to the exponential scaling one is typically limited to a few tens of
  electrons or spins. To extend the range of possible geometries I have
  developed these computations towards high-performance computing during
  my Ph.D. with Andreas Läuchli. There are two essential ingredients for
  making these simulations possible. First, Hamiltonian symmetries like
  space group symmetries and particle number conservation have to be
  exploited. For this, I developed the so-called "sublattice coding algorithm"
  which efficiently deals with a symmetry-adapted basis of the Hilbert
  space. Second, I proposed an efficient parallelization method for
  distributed memory machines by randomly distributing the basis of the
  Hilbert space. More precisely, basis configurations are hashed onto
  different MPI processes. These algorithms are described in detail in
  Ref.<d-cite key="Wietek2018"></d-cite>. I have since been using this 
  software as a basis to perform various other projects<d-cite key="Wietek2015,Wietek2017a,Wietek2020a,Chen2020,Wietek2020a"></d-cite>.
</p>

<div class="row">
    <div class="col-sm-5 mt-2 mt-md-0">
    <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/square_50.png' | relative_url }}" alt="" title="example image"/>
    </div>
    
    <div class="col-sm mt-2 mt-md-1">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/speedup.png' | relative_url }}" alt="" title="example image"/>
    </div>

</div>
<div class="caption">
   (Left) Efficient use of conservation laws and distributed memory parallelization allowed us to compute the ground state energy \( E_0 = -33.7551019315 \) of the Heisenberg model on a \(N=50\) site square lattice<d-cite key="Wietek2018"></d-cite> (Right) Strong scaling analysis of the parallelized exact diagonalization code. We observe good scaling behavior up to several thousand cores. 
</div>