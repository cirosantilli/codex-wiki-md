<h1 id="3/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

A particularly simple constructive choice uses paired [collocation points for a global relation](../../../../../../collocation-points-for-a-global-relation.md). For $n=1,\ldots,N$, put

$$
p_n=\frac{n\pi}{2},\qquad \omega_n=\sqrt{k^2+p_n^2},\qquad r_n=\frac{\omega_n+p_n}{k}>1,\qquad r_n^{-1}=\frac{\omega_n-p_n}{k}.
$$

Four suitable sets, one for each side, are

$$
\boxed{\Lambda_B=\{r_n,r_n^{-1}\},\quad\Lambda_T=\{-r_n,-r_n^{-1}\},\quad\Lambda_L=\{ir_n,i r_n^{-1}\},\quad\Lambda_R=\{-ir_n,-i r_n^{-1}\},\quad 1\leq n\leq N.}
$$

The braces in each set range over all $n$. For large $p_n/k$, compute $r_n^{-1}=k/(\omega_n+p_n)$ to avoid cancellation. The corresponding $(A,B)$ pairs are, respectively,

$$
(\pm ip_n,-\omega_n),\quad(\mp ip_n,\omega_n),\quad(-\omega_n,\mp ip_n),\quad(\omega_n,\pm ip_n).
$$

Each pair has the same exponentially growing normal direction and opposite tangential frequencies. Take the phase-weighted difference of the two collocated [global relations for a linear boundary value problem](../../../../../../global-relation-for-a-linear-boundary-value-problem.md). For example, the bottom pair gives the adjoint test

$$
v_{Bn}(x,y)=\frac{e^{ip_n}v_{r_n}-e^{-ip_n}v_{r_n^{-1}}}{2i}=e^{-\omega_ny}\phi_n(x).
$$

The other three phase-weighted differences give

$$
v_{Tn}=e^{\omega_ny}\phi_n(x),\qquad v_{Ln}=e^{-\omega_nx}\phi_n(y),\qquad v_{Rn}=e^{\omega_nx}\phi_n(y).
$$

Thus the four spectral sets supply four real sine-tested equations per mode. We retain these $4N$ equations; requiring every uncombined complex equation as well would instead form an overdetermined finite approximation. For real traces each retained equation is the appropriate real combination of its conjugate pair.

The key advantage is that $v_{Bn},v_{Tn}$ vanish on the vertical sides, while $v_{Ln},v_{Rn}$ vanish on the horizontal sides. [Orthogonality](../../../../../../orthogonal-vectors.md) then eliminates all off-mode unknowns. Define the known right-hand sides

$$
R_{jn}=\int_{\partial\Omega}f^{(M)}\partial_nv_{jn}\,ds.
$$

The retained [global relations for a linear boundary value problem](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) are

$$
\begin{pmatrix}e^{\omega_n}&e^{-\omega_n}\\e^{-\omega_n}&e^{\omega_n}\end{pmatrix}\begin{pmatrix}c_{Bn}\\c_{Tn}\end{pmatrix}=\begin{pmatrix}R_{Bn}\\R_{Tn}\end{pmatrix},\qquad
\begin{pmatrix}e^{\omega_n}&e^{-\omega_n}\\e^{-\omega_n}&e^{\omega_n}\end{pmatrix}\begin{pmatrix}c_{Ln}\\c_{Rn}\end{pmatrix}=\begin{pmatrix}R_{Ln}\\R_{Rn}\end{pmatrix}.
$$

For example, with $f_{jn}=\int_{-1}^1f_j^{(M)}(s)\phi_n(s)\,ds$, the bottom and top right-hand sides are explicitly

$$
R_{Bn}=\omega_ne^{\omega_n}f_{Bn}-\omega_ne^{-\omega_n}f_{Tn}+p_n\int_{-1}^1e^{-\omega_ns}[(-1)^nf_R^{(M)}(s)-f_L^{(M)}(s)]\,ds,
$$



$$
R_{Tn}=-\omega_ne^{-\omega_n}f_{Bn}+\omega_ne^{\omega_n}f_{Tn}+p_n\int_{-1}^1e^{\omega_ns}[(-1)^nf_R^{(M)}(s)-f_L^{(M)}(s)]\,ds.
$$

For completeness the left and right right-hand sides are

$$
R_{Ln}=\omega_ne^{\omega_n}f_{Ln}-\omega_ne^{-\omega_n}f_{Rn}+p_n\int_{-1}^1e^{-\omega_ns}[(-1)^nf_T^{(M)}(s)-f_B^{(M)}(s)]\,ds,
$$



$$
R_{Rn}=-\omega_ne^{-\omega_n}f_{Ln}+\omega_ne^{\omega_n}f_{Rn}+p_n\int_{-1}^1e^{\omega_ns}[(-1)^nf_T^{(M)}(s)-f_B^{(M)}(s)]\,ds.
$$

All these integrals use known [polynomial](../../../../../../polynomial-split.md) approximations or the exact [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md).

Scale each row by $e^{-\omega_n}$. Every block becomes

$$
\boxed{\begin{pmatrix}1&\delta_n\\\delta_n&1\end{pmatrix},\qquad \delta_n=e^{-2\omega_n}<e^{-\pi}<1.}
$$

There is just one off-diagonal entry in each row. This proves [diagonal dominance of paired square global-relation collocation](../../../../../../diagonal-dominance-of-paired-square-global-relation-collocation.md). Therefore **the assembled $4N\times4N$ system is strictly diagonally dominant**, with row margin $1-\delta_n>1-e^{-\pi}$. This proof applies to the explicitly paired and scaled collocation system, rather than assuming arbitrary raw spectral rows are diagonally dominant. Each block is a [positive-definite matrix](../../../../../../positive-definite-matrix.md) and have [spectral condition number of a positive-definite matrix](../../../../../../spectral-condition-number-of-a-positive-definite-matrix.md)

$$
\kappa_2=\frac{1+\delta_n}{1-\delta_n}<\frac{1+e^{-\pi}}{1-e^{-\pi}}<1.091.
$$

For instance, setting $\rho_{jn}=e^{-\omega_n}R_{jn}$ gives the concise answer

$$
\boxed{c_{Bn}=\frac{\rho_{Bn}-\delta_n\rho_{Tn}}{1-\delta_n^2},\qquad c_{Tn}=\frac{\rho_{Tn}-\delta_n\rho_{Bn}}{1-\delta_n^2},}
$$

with the identical formula for the opposite vertical sides. If the known-data integrals use exact $f_j$, these are exactly the first $N$ sine coefficients of the true normal traces: no discarded unknown mode contributes to a retained row. With a finite [Legendre polynomial](../../../../../../legendre-polynomial.md) approximation, the error is solely that of the known-data approximation and the final normal-trace truncation. These [square modified Helmholtz Dirichlet-to-Neumann coefficients](../../../../../../square-modified-helmholtz-dirichlet-to-neumann-coefficients.md) determine the unknown boundary [normal derivative](../../../../../../normal-derivative.md); [Green's third identity](../../../../../../green-s-third-identity.md) or the separated-variable construction can then recover the interior solution.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [3](../../3.md)
3. [Paper 328](../../../paper-328-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
