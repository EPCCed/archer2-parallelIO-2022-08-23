<img src="./images/Archer2_logo.png" width="355" height="100"
align="left"> <img src="./images/epcc_logo.jpg" align="right"
width="133" height="100">

<br /><br /><br /><br /><br />

# Efficient Parallel IO on ARCHER2 

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

<h3>David Henty EPCC: Tuesday 23rd August 2022, 09:30 - 16:30 GMT, online</h3>

One of the greatest challenges to running parallel applications on
large numbers of processors is how to handle file IO. Standard Unix IO
routines are not designed with parallelism in mind, and IO overheads
can grow to dominate the overall runtime. Parallel file systems are
optimised for large volumes of data, but performance can be far from
optimal if every process opens its own file or if all IO is funnelled
through a single controller process.

This hands-on course explores a range of issues related to parallel
IO. It uses ARCHER2 and its parallel Lustre file system as a platform
for the exercises; however, almost all the IO concepts and performance
considerations are applicable to any parallel system.

We will give a general overview of the Lustre filesystem and how
parallel IO is implemented in MPI-IO since these are the routines
ultimately used by many higher-level libraries such as HDF5 and
NetCDF. A good understanding of the performance characteristics of
MPI-IO is therefore very useful in optimising the IO performance of
most parallel applications.

The course does not teach the detailed syntax of the various parallel
IO libraries, but the Fortran source code provided for the
benchmarking application used in the practical sessions should be
useful reference material.

<h3>Prerequisites</h3>

Prerequisites: The course assumes an understanding of basic MPI
programming in C, C++ or Fortran. Knowledge of MPI derived datatypes
would be useful but not essential.

<h3>Requirements</h3>

Participants must bring a laptop with a Mac, Linux, or Windows
operating system (not a tablet, Chromebook, etc.) that they have
administrative privileges on.

They are also required to abide by the [ARCHER2 Code of Conduct](https://www.archer2.ac.uk/about/policies/code-of-conduct.html).

<h3>Timetable (all times are in GMT)</h3>

<p><blockquote>Unless otherwise indicated all material is Copyright
&copy; EPCC, The University of Edinburgh, and is only made available
for private study. </blockquote></p>

<h4>Tuesday 11th January</h4>

 * 09:30 - 10:15 : <a href="https://github.com/EPCCed/archer2-parallelIO-2022-01-11/raw/main/slides/Parallel-IO-1.pdf">Challenges of Parallel IO</a>
 * 10:15 - 10:45 : <a href="https://github.com/EPCCed/archer2-parallelIO-2022-01-11/raw/main/slides/Parallel-IO-2.pdf">Lustre file system on ARCHER2</a>
 * 10:45 - 11:00 : Practical: Basic IO performance
 * 11:00 - 11:30 : Break
 * 11:30 - 12:00 : Practical: Basic IO performance (cont)
 * 12:00 - 12:45 : <a href="https://github.com/EPCCed/archer2-parallelIO-2022-01-11/raw/main/slides/Parallel-IO-3.pdf">Overview of MPI-IO</a>
 * 12:45 - 13:00 : Practical: MPI-IO performance
 * 13:00 - 14:00 : Lunch
 * 14:00 - 14:30 : <a href="https://github.com/EPCCed/archer2-parallelIO-2022-01-11/raw/main/slides/Parallel-IO-4.pdf">Configuring the Lustre filesystem</a>
 * 14:30 - 15:00 : Practical: MPI-IO performance (cont)
 * 15:00 - 15:30 : <a href="https://github.com/EPCCed/archer2-parallelIO-2022-01-11/raw/main/slides/Parallel-IO-5.pdf">Higher-level parallel IO libraries</a>
 * 15:30 - 16:00 : Break
 * 16:00 - 16:30 : Q&A / Finish exercises
 * 16:30         : CLOSE

<h3>Exercise Material</h3>

<p><blockquote>Unless otherwise indicated all material is Copyright
&copy; EPCC, The University of Edinburgh, and is only made available
for private study. </blockquote></p>

<p><blockquote>This is still a draft course page and the material
below comes from a previous run of this course. It will be updated for
this run, but is made available here for reference.</blockquote></p>

Here is the <a href="https://github.com/EPCCed/archer2-parallelIO-2022-01-11/raw/main/exercises/benchio-archer2.pdf">parallel IO exercise sheet.</a>. As explained in the sheet, source code and instructions for the IO benchmark can be found at <a href="https://github.com/davidhenty/benchio">https://github.com/davidhenty/benchio/.</a>

---

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

