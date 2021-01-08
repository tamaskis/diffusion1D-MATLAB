# `diffusion1D`

Solves the one-dimensional diffusion equation (i.e. heat equation) for Neumann and Dirichlet type boundary conditions.


## Syntax

`[x,f,Fo] = diffusion1D(sol_method,D,L,N,IC,g_func,gType,h_func,hType,dt,tmax)`


## Description

`[x,f,Fo] = diffusion1D(sol_method,D,L,N,IC,g_func,gType,h_func,hType,dt,tmax)` returns the solution of the diffusion equation at time <img src="https://latex.codecogs.com/svg.latex?t_{\mathrm{max}}" title="t_{\mathrm{max}}" /> (as the vector `f`), as well as the spatial domain for the solution (`x`) an the discrete Fourier number (`Fo`).
- `sol_method` - solution method (`FTCS_looped` for looped FTCS, `FTCS_simultaneous` for simultaneous FTCS, `BTCS` for BTCS, and `CTCS` for CTCS (Crank-Nicolson))

`X = rand2(a,b,[m,n])` returns an <img src="https://latex.codecogs.com/svg.latex?m\times&space;n" title="m\times n" /> matrix of random double-precision floating-point numbers between <img src="https://latex.codecogs.com/svg.latex?a" title="a" /> and <img src="https://latex.codecogs.com/svg.latex?b" title="b" />.

`X = rand2(__,typename)` returns an array of random numbers of data type `typename`. The `typename` input can be either `'int'`, `'single'`, or `'double'`. You can use any of the input arguments in the previous syntaxes.
- `'int'` specifies integers
- `'single'` specifies single-precision floating-point numbers
- `'double'` specifies double-precision floating-point numbers (this specification does not have to be used; `rand2` defaults to `'double'` if no `typename` is specified)
