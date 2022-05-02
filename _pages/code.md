---
layout: page
permalink: /code/
title: Code
description: 
nav: true
order : 3
---

I am developing several software packages and am starting to make them publicly available as open-source projects. My philosophy is to continuously single out useful small modules from the larger research software I am using.

<hr>
<h4 class="card-title">ED Basics</h4>
<p class="card-text">
A minimalistic code performing Exact Diagonalization written in python. It demonstrates the basics of how to build a Hilbert space, employ space group symmetries, and iteratively compute extremal eigenvalues. The code was part of a hands-on-session I held at the FOR1809 Winter School in Marburg in 2018. 
</p>
<p style="text-align:left;">
   <a href="https://github.com/awietek/ed_basics"> Github </a>
       <span style="float:right;">
       <img height=30px src="{{ '/assets/img/python-logo.png' | relative_url }}" margin=10px>	
    </span>
</p>


<hr>
<h4 class="card-title">LiLA</h4>
<p class="post-description">Lightweight Linear Algebra</p>
<p class="card-text">
Performing elementary linear algebra operations in C++ is unfortunately not as straightforward as in other languages. There exist several good options, like Eigen or Armadillo, but these libraries are rather extensive. With this project, I provide an easy-to-use minimalistic linear algebra library by wrapping the Blas/Lapack, Intel MKL, or Accelerate subroutines.
</p>
<p style="text-align:left;">
   <a href="https://github.com/awietek/lila"> Github </a>
    <span style="float:right;">
       <img height=30px src="{{ '/assets/img/cpp-logo.svg' | relative_url }}" margin=10px>	
    </span>
</p>

<hr>
<h4 class="card-title">LiMe</h4>
<p class="post-description">Lightweight Measurements</p>
<p class="card-text">
The hdf5 data format is a modern standard for scientific data sets. Its C interface is versatile, but not straightforward to use. This software project provides an intuitive C++ interface for writing scalars, vectors, and matrices to an hdf5 file, without having to deal with low-level function calls. The package also features extensible data collection, which is useful when consecutive measurements (from e.g. a Monte Carlo simulation) have to be accumulated.
</p>

<p style="text-align:left;">
    <a href="https://github.com/awietek/lime"> Github </a>
    <span style="float:right;">
       <img height=30px src="{{ '/assets/img/cpp-logo.svg' | relative_url }}" margin=10px>
       <img height=25px src="{{ '/assets/img/HDF_logo.svg' | relative_url }}" margin=10px>	
    </span>
</p>

<hr>
<h4 class="card-title">Hydra</h4>
<p class="card-text">
An Exact Diagonalization software package where elementary operations are parallelized for distributed memory machines. The code is designed to scale Hamiltonian matrix-vector multiplications up to several thousand cores on modern supercomputers. The design principles are described in <a href="https://journals.aps.org/pre/abstract/10.1103/PhysRevE.98.033309">this paper</a>. 
Currently, it is available for collaborators only.
</p>

<p style="text-align:left;">
   <a href="https://github.com/awietek/hydra"> Github </a>
    <span style="float:right;">
       <img height=30px src="{{ '/assets/img/cpp-logo.svg' | relative_url }}" margin=10px>
       <img height=25px src="{{ '/assets/img/MPIlogo.gif' | relative_url }}" margin=10px>	
    </span>
</p>
