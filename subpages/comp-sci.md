---
layout: page
permalink: comp-sci
---

# Computational Science <!-- omit in toc -->

---

- [Chatbot](https://sites.google.com/site/rangsiman1993/comp-env/comp-sci/chatbot)
- [Machine Learning: Iris as a case study](https://sites.google.com/site/rangsiman1993/comp-env/comp-sci/machine-learning-iris)
- [Microsoft Imagine Premium for Student and Lecturer](https://sites.google.com/site/rangsiman1993/comp-env/comp-sci/microsoft-imagine-premium-for-education)

---

<br>

# Skills Checklist <!-- omit in toc -->

- [General technical skills](#general-technical-skills)
- [Computer Science Skills](#computer-science-skills)
- [Essential skills for software development](#essential-skills-for-software-development)
- [Essential skills for HPC](#essential-skills-for-hpc)
- [Essential skills for coding GPU](#essential-skills-for-coding-gpu)
- [Essential skills for machine learning (bonus)](#essential-skills-for-machine-learning-bonus)

<br>

## General technical skills

- For Windows:
  - Install programs and modify system variables
  - Install Nvidia CUDA toolkit and driver
  - Setup VPN and local network
  - Setup dual boost for Linux, or install WSL for Ubuntu
- For Linux and macOS:
  - Basic/intermediate commands
  - Know some important files/folders
  - Understand some environmen variables
- Scripting programming language
  - Bash, awk, perl, Python + Jupyter notebook
- Cluster / HPC
  - Understand terminology: master node, compute node, scheduler, CPU cores, processes, memory
  - Scheduler: Slurm, PBS, SGE
  - Software manager: module
- Software
  - Commercial: Gaussian, Q-Chem, ADF, MOLPRO, MOLCAS, TURBOMOLE and many more
  - Non-commercial: PySCF, Psi4, OpenMOLCAS, GAMESS, ORCA, NWChem, DIRAC, DALTON, CP2K, LAMMPS, VASP, QE and many more
  - Full list is [here](https://en.wikipedia.org/wiki/List_of_quantum_chemistry_and_solid-state_physics_software)
- Graphic visualization
  - JMol, Molden, Gaussview, Avogadro, UCSF Chimera, VMD, Ovito, PyMol
  - 2D and 3D plots
- Other useful tools
  - ASE, MDTraj, Pymatgen, RDKit, OpenBabel
- Writing
  - Microsoft Word
  - LaTeX
    - Compiler: pdflatex, xelatex, lualatex
    - Distribution: TeX Live, MikTeX
    - Editor: OverLeaf, TeXstudio, Texmaker
- Presentation
  - Powerpoint
  - LaTeX Beamer

## Computer Science Skills

- Programming (Python, C++, etc.)
- Scientific Computing
- Scientific Programming in Python
- High Performance Computing
- Computer Applications in Chemistry, Biology, and Physics
- Programming in C++
- Algorithm in Software Development
- Interdisciplinary Research Methods In Computational Biology
- Data Analysis in Biology
- Introduction to Machine Learning
- Introduction to Deep Learning
- Neural Network and Computer Vision

## Essential skills for software development

- Tex editor
  - Vi/Vim, Nano
  - VS Code, Atom, Eclipse, Sublime
- File format
  - XML, JSON
- General programming skills
  - Type of variables
  - Loops and conditional statement
  - Input/output
- High-level programming
  - Python
    - Pip and conda: Python helper
    - NumPy: Array (vector, matrix) computation
    - Numba: JIT compiler for NumPy
    - Jax: autograd of NumPy array
    - SciPy: a collection of math functions/routines
    - Scikit-learn: statistics routines, optimization, curve fitting
      - Intel Scikit-learn is 10x faster than the standard one
    - Matplotlib / Plotly for plotting graph
    - Theano: numerical computation
    - SCOOP: distributed modules for parallel programming
    - NetworkX: Graph library
- Low-level programming
  - C
    - Function, pointer, storage class
    - Enum, struct, union
    - Preprocessor
    - Operator, memory management, array
    - File handling
  - C++
    - C++ 11 or newer
    - Type of variable: signed, unsigned, long, double, etc.
    - Loops, conditional statement
    - Standard libraries: vector, rand
    - Understanding header and source file
    - Preprocessor
    - Function, class, struct, template
    - Declaration
      - namespace, const, attribute, pointer, pass by reference, static_assert
    - Initialization
    - Misc: casting, lambda expression, encapsulation, file handling, exception handling
  - Fortran
    - Learn either F77 or F90 or modern fortran (2003, 2008, 2018)
    - Module, subroutine, function
    - Array (allocatable and multidimentional) and string
    - Operator overloading
    - Flow control
    - Derived type
    - Callback
    - Interfacing to other language e.g. Python or C++
  - GNU library
    - GSL
    - Many more libraries [here](https://en.wikipedia.org/wiki/List_of_GNU_packages)
- Memory allocation
  - Stack, heap, global memory
- Math libraries
  - BLAS (OpenBLAS)
  - LAPACK for linear algebra
  - ScaLAPACK - a higher level LAPACK
  - Intel MKL (Intel oneAPI)
  - FFTW: for computing the discrete Fourier transform in one or more dimensions, real and complex data
  - Eigen: linear algebra library
  - Boost: a collection of C++ functions
- QM libraries
  - libxc: XC function library
  - libint: For computing Gaussian integral
  - libcint: general GTO integrals
- Code optimization
  - Benchaming/scaling
  - Complexity (Big O)
- GNU
  - Static and dynamic libraries
  - Archive
  - Compiling (g++, gcc) and linking (ld)
  - Useful flags for compiler and linker
- Compilng tools
  - autoconf
  - configure
  - Make, cmake, automake
- Debugging
  - gdb for general debugging
  - Valgrind for memory leak analysis
- Git (source code control)
  - Basic/intermediate commands
  - GitHub & GitLab
- Documentation
  - Sphinx (for markdown and reStructuredText)
  - Doxygen

## Essential skills for HPC

- Architecture
  - Memory management
  - Threading, multithreading
  - Block
- Parallel computing (SPMD)
  - Shared memory: OpenMP
  - Distributed memory: MPI
    - Implementations: OpenMPI, Intel MPI, MVAPICH
- Intel ecosystem
  - OpenMP compiler: icc, ifort
  - MPI compiler: mpicc, mpiicc (for Intel C compiler), mpicxx (for C++), mpiifort (for Fortran)
- Cloud computing (bonus)
- Server and database
- Networking

## Essential skills for coding GPU

- Intermediate/advanced C or C++ skills
- Programming model: Kernels, thread hierarchy, memory hierarchy, heterogeneous hierarchy, asynchronous SIMT
- CUDA
  - Understand CUDA operation:
    1. Declare and allocate host and device memory.
    2. Initialize host data.
    3. Transfer data from the host to the device.
    4. Execute one or more kernels.
    5. Transfer results from the device to the host.
  - CUDA C and CUDA C++ API
  - Compiler: nvcc

## Essential skills for machine learning (bonus)

- Basic math: linear algebra and calculus
- Programming
  - Python, R, Julia, Matlab
  - TensorFlow, PyTorch, Scikit-learn
- Python lib
  - NumPy
  - Pandas
- Terminology: regression, classification, descriptor, feature, kernel, activation function
- Data analysis/engineering: EDA, ETL
- Graphical representation
  - Histogram, bar plot, heatmaps
- ML algorithms
  - Decision tree
  - Random forest
  - Support vector machine
  - Principal component analysis
  - Kernel-ridge method
  - Neural network
    - Feedforward NN
      - Autoencoder
    - CNN
    - RNN (LSTM)
    - GNN
    - Adversarial NN
      - GAN
- Model training and optimization
  - Hyperparameter optimization
- Techniques to prevent overfittingTechniques
  - Data augmentation, early stopping, regularization, dropout, batch normalization
- Deploying model
