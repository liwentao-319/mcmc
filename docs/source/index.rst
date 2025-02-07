.. Copyright (c) 2011-2022 Keith O'Hara

   Distributed under the terms of the Apache License, Version 2.0.

   The full license is in the file LICENSE, distributed with this software.

Introduction
============

MCMCLib is a lightweight C++ library of Markov Chain Monte Carlo (MCMC) methods.

Features:

- A C++11/14/17 library of well-known MCMC algorithms.

- Parallelized samplers designed for multi-modal distributions, including:
  
  - Differential Evolution (DE); and

  - Adaptive Equi-Energy Sampler (AEES).

- For fast and efficient matrix-based computation, MCMCib supports the following templated linear algebra libraries:

  - `Armadillo <http://arma.sourceforge.net/>`_ 

  - `Eigen <http://eigen.tuxfamily.org/index.php>`_ (version >= 3.4.0)

- Automatic differentiation functionality is available through use of the `Autodiff library <https://autodiff.github.io>`_

- OpenMP-accelerated algorithms for parallel computation. 

- Straightforward linking with parallelized BLAS libraries, such as `OpenBLAS <https://github.com/xianyi/OpenBLAS>`_.

- Available as a header-only library, or as a compiled shared library.

- Released under a permissive, non-GPL license.

Author: Keith O'Hara

License: Apache Version 2.0

----

Installation
------------

The library can be installed on Unix-alike systems via the standard ``./configure && make`` method.

See the installation page for :ref:`detailed instructions <installation>`.

Algorithms
----------

A list of currently available algorithms includes:

* Random Walk Metropolis-Hastings (RWMH)
* Hamiltonian Monte Carlo (HMC)
* Riemannian Manifold Hamiltonian Monte Carlo (RM-HMC)
* Metropolis-adjusted Langevin algorithm (MALA)
* Adaptive Equi-Energy Sampler (AEES)
* Differential Evolution (DE-MCMC)

----

Contents
--------

.. toctree::
   :caption: Guide
   :maxdepth: 2
   
   installation
   examples_and_tests
   settings
   autodiff

.. toctree::
   :caption: Algorithms
   :maxdepth: 1
   
   api/aees
   api/de
   api/hmc
   api/mala
   api/rwmh
   api/rmhmc

.. toctree::
   :caption: Appendix
   :maxdepth: 2
   
   box_constraints
