<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

After spatial discretization, a linear time-dependent PDE produces an update

$$
u^{n+1}=Q_hu^n.
$$

Stability over $0\leq n\Delta t\leq T$ requires a bound $\lVert Q_h^n\rVert\leq C_T$ independent of the mesh. If $Q_h$ is normal, the [spectral theorem for normal operators](../../../../../spectral-theorem-for-normal-operators.md) gives

$$
\lVert Q_h^n\rVert_2=\max_j|\lambda_j(Q_h)|^n,
$$

so eigenvalue analysis is decisive. More generally, if $Q_h=X_h\Lambda_hX_h^{-1}$, then

$$
\lVert Q_h^n\rVert\leq
\kappa(X_h)\max_j|\lambda_j|^n.
$$

Thus eigenvalues suffice only when the eigenvector condition numbers are uniformly bounded and unit-circle eigenvalues are semisimple. Defective or increasingly nonnormal matrices can have large powers even though every eigenvalue lies in the unit disk.

For a constant-coefficient scheme on the whole line or a periodic grid, the [discrete Fourier transform](../../../../../discrete-fourier-transform.md) diagonalizes translation-invariant difference operators. This is [von Neumann stability analysis](../../../../../von-neumann-stability-analysis.md): insert $u_m^n=G(\theta)^ne^{im\theta}$ and require $|G(\theta)|\leq1$. Its advantages are simplicity, sharp mesh restrictions, and direct identification of unstable wavelengths. Its limitations are boundaries, variable coefficients, nonlinearities, and nonnormality; frozen-coefficient Fourier analysis then gives at most local evidence.

As a successful implicit example, the [Backward Euler diffusion scheme](../../../../../backward-euler-diffusion-scheme.md) has

$$
Q_h=(I-\Delta tD_h)^{-1},
$$

where the periodic or homogeneous-Dirichlet discrete Laplacian $D_h$ is symmetric negative semidefinite. Its eigenvalues are $(1-\Delta t\lambda_j(D_h))^{-1}\in(0,1]$, proving unconditional discrete-$2$-norm stability.

For a failure, consider explicit upwinding for $u_t+a u_x=0$ on a finite inflow grid:

$$
u_j^{n+1}=(1-\mu)u_j^n+\mu u_{j-1}^n,
\qquad u_0^n=0.
$$

Its lower-triangular [nonnormal upwind amplification matrix](../../../../../nonnormal-upwind-amplification-matrix.md) has only the eigenvalue $1-\mu$, so eigenvalues alone incorrectly suggest stability for $0\leq\mu\leq2$. For $1<\mu<2$, however, interior alternating data are amplified by $|1-2\mu|>1$ before the boundary is felt, and the matrix powers have no mesh-uniform bound. The correct range is $0\leq\mu\leq1$. This example isolates the missing hypothesis: spectral radius does not control powers of a nonnormal matrix family.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 341](../../paper-341-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
