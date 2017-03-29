TADGENS
=======

A Taylor-basis discontinuous Galerkin solver for compressible flow problems. See ./doc/theory for a description of the method used.

Building
--------
A CMake build system is used. GCC g++ is the compiler regularly built against, but clang++ is theoretically supported as well.

Running
-------
The executables should be called with the path to a control file as input. Note that in control files, the locations of mesh files and output files should be relative to the directory from which the executable is called.

Roadmap (in order of priority)
------------------------------
- Explicit TVD RK time-stepping scheme for both steady and unsteady inviscid flow problems with smooth solutions
- Reconstruction DG scheme for cost-effective higher-order accuracy
- P-multigrid scheme with explicit smoothers for steady problems
- P-multigrid scheme with implicit smoother at P0 level for steady problems
- Viscous fluxes for compressible viscous flow
- High-order implicit time-stepping in physical time coupled with p-multigrid in pseudo time


Copyright 2017 Aditya Kashi. See LICENSE.md for terms of redistribution with/without modification and those of linking.
Note that the license does not apply to the Eigen library, which is distributed herein without modifications. The original licensing terms apply to it; see the COPYING files in the eigen-3.3.3 directory.
