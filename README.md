
<h1 align="center">
  <br>
  OS Lab CEP
  <br>
</h1>

<h4 align="center">Threading/Parallelization</h4>
<h3 align="center"><b>Parallelized implementation of Gauss-Seidel 
method using OpenMP and POSIX Threads</b></h3>

<p></p>
<p align="center">

  <a href="#">
		<img src="https://forthebadge.com/images/badges/made-with-c.svg" alt=" Made with Python.">
  </a>

</p>

<p align="center">
  <a href="#about">About</a> •
  <a href="#report">Report</a>
</p>

<hr>

## About

This program solves a partial differential equation on (N+2) × (N+2) grid (2D), in a parallel fashion; that is, it performs Gauss-Seidel sweeps over the grid until convergence.

Two solutions are explored in this program, namely:
* Red-Black Cells Approach
* Anti-Diagonals Approach

In each case, the following parallelization techniques were tried out and the results were compared:
* Sequential Implementation
* Parallel Implementation with <b>OpenMP</b>
  - using <i>#pragma omp critical</i>
  - using per-thread <i>diff</i> variable (no padding)
  - using per-thread <i>diff</i> variable (with padding)
* Parallel Implementation with <b>Pthreads (POSIX Threads)</b>
  - using mutex lock
  - using per-thread <i>diff</i> variable (no padding)
  - using per-thread <i>diff</i> variable (with padding)


See the <a href="#report">report.pdf</a> document below for further details. 

## Report

<object data="report.pdf" type="application/pdf" width="700px" height="700px">
    <embed src="report.pdf">
        <p>This browser does not support PDFs. Please <a href="https://github.com/kamiljaved98/OS-Lab_CEP/raw/master/report.pdf">download</a> the PDF to view it.</p>
    </embed>
</object>


---

> [kamiljaved.pythonanywhere.com](https://kamiljaved.pythonanywhere.com/) &nbsp;&middot;&nbsp;
> GitHub [@kamiljaved98](https://github.com/kamiljaved98)