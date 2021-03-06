# Poisson-solver-2D



<p float="left">
<a href = "https://github.com/zaman13/Particle-Swarm-Optimization-Fortran-95/tree/master/Fortran%20codes"> <img src="https://img.shields.io/badge/Language-Python-blue" alt="alt text"> </a>
<a href = "https://github.com/zaman13/Poisson-solver-2D/blob/master/LICENSE"> <img src="https://img.shields.io/github/license/zaman13/Poisson-solver-2D" alt="alt text"></a>
<a href = "https://github.com/zaman13/Poisson-solver-2D/tree/master/Code"> <img src="https://img.shields.io/badge/version-1.1-red" alt="alt text"> </a>
</p>

<p>
Finite difference solution of 2D Poisson equation <img src="https://render.githubusercontent.com/render/math?math=\nabla^2u(x,y) = g(x,y)">

<img align = "right" src="https://github.com/zaman13/Poisson-solver-2D/blob/master/Laplace_figure_output_2.png"  width = "440">

Current version can handle Dirichlet boundary conditions:

<img src="https://render.githubusercontent.com/render/math?math=u(x=x_L,y) = u_L">  (left boundary value)

<img src="https://render.githubusercontent.com/render/math?math=u(x=x_R,y) = u_R">  (right boundary value)

<img src="https://render.githubusercontent.com/render/math?math=u(x,y=y_T) = u_T">  (Top boundary value)

<img src="https://render.githubusercontent.com/render/math?math=u(x,y=y_B) = u_B">  (Bottom boundary value)
  
</p>

The boundary values themselves can be functions of (x,y).

### Package requirements
  - NumPy 
  - SciPy (sparse matrices, sparse linear algebra) <a href = "https://docs.scipy.org/doc/scipy/reference/sparse.html"> <img src="https://img.shields.io/badge/Pkg-sparse-yellow" alt="alt text"> </a> <a href = "https://docs.scipy.org/doc/scipy/reference/sparse.linalg.html"> <img src="https://img.shields.io/badge/Pkg-sparse.linalg-yellow" alt="alt text"> </a>


### Version notes
- version 1.1
  - Fixed a bug regarding the right-hand function
  - Figure size and font size adjusted

- version 1.0 notes
  - Sparse matrix implementation. CSR format (Compressed sparse row matrix) matrix.

### Sample Output
Solution of <img src="https://render.githubusercontent.com/render/math?math=\nabla^2u(x,y) = 0"> with boundary conditions <img src="https://render.githubusercontent.com/render/math?math=u(-6,y) = 0.5, u(6,y) = 1.2, u(x,-3) = -0.75, u(x,3) = -1"> is shown below:

 <img src="https://github.com/zaman13/Poisson-solver-2D/blob/master/Laplace_figure_output.png"  width = "400">

### References
  - Sparse matrices: https://docs.scipy.org/doc/scipy/reference/sparse.html
  - Sparse matrix linear algebra: https://docs.scipy.org/doc/scipy/reference/sparse.linalg.html
