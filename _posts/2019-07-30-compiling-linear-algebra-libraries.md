---
layout: post
title: Compiling Powerful Linear Algebra Libraries on Linux
author: Rangsiman Ketkaew
date: "2019-07-30 00:12:00 +0700"
category:
  - library
  - environment
  - math
  - installation
  - software
summary: Compiling powerful linear algebra libraries on Linux
thumbnail: posts/linalg.png
permalink: content/8
comments: true
---

## Table of Content

- [Table of Content](#table-of-content)
- [Compiling Linear Algebra Libraries](#compiling-linear-algebra-libraries)
- [Linear algebra software I am installing are following](#linear-algebra-software-i-am-installing-are-following)
- [Caveat](#caveat)
- [BLAS](#blas)
- [LAPACK](#lapack)
- [CBLAS](#cblas)
- [ScaLAPACK](#scalapack)
- [ATLAS](#atlas)
- [Error while compiling ATLAS](#error-while-compiling-atlas)
- [MKL](#mkl)

<br>

## Compiling Linear Algebra Libraries

This post will show how to compile and install linear algebra libraries such as BLAS and LAPACK on Linux-based operating system step-by-step. These linear algebra mathematical libraries have been generously used in computational science and development for compiling a mid- and top-level scientific programming such as Fortran, C, and C++ programming languages.

<br>

## Linear algebra software I am installing are following

* Basic Linear Algebra Subprogram (BLAS)
* Linear Algebra Package (LAPACK)
* C/C++ interface to BLAS (CBLAS)
* Scalable Linear Algebra PACKage (ScaLAPACK)
* Automatically Tuned Linear Algebra Soft (ATLAS)
* Intel Math Kernel Library (MKL)

Their latest versions can be obtained from Netlib Repository: <http://www.netlib.org/liblist.html>, except ATLAS, which its latest version is available at <https://sourceforge.net/projects/math-atlas/files/Stable/> as well as Intel MKL that available only at Intel software suite website.

<br>

## Caveat

1. I use GNU Compiler and OpenMPI of writing this post.
2. I install all libraries in home directory (/home/rangsiman/).

<br>

## BLAS

See [LAPACK](#lapack)

<br>

## LAPACK

Due to a low-level BLAS software is part of LAPACK, thus I installed only LAPACK. No need to install BLAS separately.

1. Download tarball of LAPACK from this website <http://www.netlib.org/lapack/>.

2. There will be LAPACK directory called lapack-3.8.0. (the current version of this writing)

3. Move to LAPACK directory
```
cd lapack-3.8.0
```

4. Create make.inc by copying from makefile.inc.example, which is a standard one.
```
cp make.inc.example make.inc
```

5. Compile and Install using Makefile.
```
make blaslib
make
```

6. After installation is finished, there must be three libraries in LAPACK directory:
* liblapack.a
* librefblas.a
* libtmglib.a

7. Create symbolic link of librefblas.a as libblas.a library.
```
ln -s librefblas.a libblas.a
```

<br>

## CBLAS

A **libblas.a** library is required for compiling CBLAS

1. Download the tar.gz. file of CBLAS from BLAS forum on Netlib repository to your Linux <http://www.netlib.org/blas/index.html#_cblas>.

2. Unpack the tar file using following command
```
tar -xzvf cblas.tgz
```

3. Move to CBLAS directory
```
cd CBLAS
```

4. Edit PATH of libblas.a and name of CBLAS library at line 26 and 27 in **Makefile.in** file
```
vi Makefile.in
BLLIB = /home/rangsiman/lapack-3.8.0/libblas.a
CBLIB = ../lib/libcblas.a
```
Note that a **libblas.a** static library can be obtained from LAPACK directory, where you installed in previous section.

5. Install CBLAS using make
```
make
```

6. After installation is completed, there must be **libcblas.a** in **CBLAS/lib** sub-directory.

<br>

## ScaLAPACK

1. Download the tar.gz. file of ScaLAPACK from Netlib repository to your Linux <http://www.netlib.org/scalapack/#_software>

2. Unpack the tar file using following command
```
tar -xzvf scalapack-2.0.2.tgz
```

3. Move to ScaLAPACK directory
```
cd scalapack-2.0.2
```

4. Copy SLmake.inc.example to SLmake.inc.
```
cp SLmake.inc.example SLmake.inc
```

5. Install ScaLAPACK using make
```
make
```
This can take several minutes.

6. After installation is completed, there must be libscalapack.a in ScaLAPACK directory.

<br>

## ATLAS

I am going to install ATLAS under my home directory as normal user.


1. Uncompress tarball 
```
mv tlas3.8.3.tar.gz $HOME/
cd $HOME
tar -xzvf atlas3.8.3.tar.gz
```

2. Create new directory (either inside or outside ATLAS directory), for example, ATLAS_BUILD
```
mkdir $HOME/ATLAS_BUILD
```

3. Move to ATLAS_BUILD directory and run configure script (from ATLAS directory) to set up compilation configuration.
```
cd $HOME/ATLAS_BUILD
../ATLAS/configure
```

4. Compile ATLAS using following commands*
```
make
```
You may run compilation using parallel making, says use 8 processors
```
make -j 8
```
This step can take several minutes/hours (depending on your computer performance).

5. Then check library before install
```
make check
make ptcheck
make time
```
If having many error occur while checking program, you might ignore those error and proceed next step.

6. Install software
```
make install
```
When installation is finished (with or without error), please check if there is linear algebra library of CBLAS, LAPACK, and ATLAS at *$HOME/ATLAS_INSTALL/lib/*.

7. Done

<br>

## Error while compiling ATLAS

There is two error that most users frequently face when install ATLAS using make install command.

1. Cannon create _/usr/local/atlas_
The default setting of target directory of compiled ATLAS library is _/usr/local/atlas_. If you are not root or sudo, you cannot install anything on global shared space. Thus you should tell make to install ATLAS under your home directory. Refer to a Makefile file at line 3, for example, change
```
DESTDIR=/usr/local/atlas
```
to
```
DESTDIR=/home/rangsiman/ATLAS_INSTALL
```

2. Cannot find some libraries
```
cp: cannot stat ‘/home/rangsiman/ATLAS_BUILD/lib/libsatlas.dylib’: No such file or directory
make[1]: [install_lib] Error 1 (ignored)
cp /home/rangsiman/ATLAS_BUILD/lib/libtatlas.dylib /home/rangsiman/ATLAS_INSTALL/lib/.
cp: cannot stat ‘/home/rangsiman/ATLAS_BUILD/lib/libtatlas.dylib’: No such file or directory
make[1]: [install_lib] Error 1 (ignored)
cp /home/rangsiman/ATLAS_BUILD/lib/libsatlas.dll /home/rangsiman/ATLAS_INSTALL/lib/.
cp: cannot stat ‘/home/rangsiman/ATLAS_BUILD/lib/libsatlas.dll’: No such file or directory
make[1]: [install_lib] Error 1 (ignored)
cp /home/rangsiman/ATLAS_BUILD/lib/libtatlas.dll /home/rangsiman/ATLAS_INSTALL/lib/.
cp: cannot stat ‘/home/rangsiman/ATLAS_BUILD/lib/libtatlas.dll’: No such file or directory
make[1]: [install_lib] Error 1 (ignored)
cp /home/rangsiman/ATLAS_BUILD/lib/libsatlas.so /home/rangsiman/ATLAS_INSTALL/lib/.
cp: cannot stat ‘/home/rangsiman/ATLAS_BUILD/lib/libsatlas.so’: No such file or directory
make[1]: [install_lib] Error 1 (ignored)
cp /home/rangsiman/ATLAS_BUILD/lib/libtatlas.so /home/rangsiman/ATLAS_INSTALL/lib/.
cp: cannot stat ‘/home/rangsiman/ATLAS_BUILD/lib/libtatlas.so’: No such file or directory
make[1]: [install_lib] Error 1 (ignored)
make[1]: Leaving directory `/home/u7/rangsiman/ATLAS_BUILD'
```
These error massages can be ignored as long as the static libraries of linear algebra software are build successfully.
All library files should be stored at 
```
/home/rangsiman/ATLAS_INSTALL/lib/
```

<br>

## MKL

Intel MKL provides a suite of ready-to-use math libraries including optimized linear algebra and Fast Fourier Transforms (FFT). Qualified student or educator and open-source software developer can obtain Intel MKL free of charge from <https://software.intel.com/en-us/mkl>.

The feature of MKL includes

* [Linear Algebra](https://software.intel.com/en-us/mkl/features/linear-algebra)
* [Fast Fourier Transforms](https://software.intel.com/en-us/mkl/features/fft)
* [Deep Neural Networks](https://software.intel.com/en-us/mkl)
* [Vector Statistics & Data Fitting](https://software.intel.com/en-us/mkl/features/statistics)
* [Vector Math & Miscellaneous Solvers](https://software.intel.com/en-us/mkl/features/vector-math-misc-solvers)
* [Performance Benchmarks](https://software.intel.com/en-us/mkl/features/benchmarks)
