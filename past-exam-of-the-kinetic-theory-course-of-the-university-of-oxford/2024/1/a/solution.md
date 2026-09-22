<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $z_i=(\mathbf x_i,\mathbf v_i)$ and $dz_i=d^3x_i\,d^3v_i$. Normalize the symmetric $N$-particle [phase-space distribution function](../../../../phase-space-distribution-function.md) $D_N$ to one. Use factorial normalization for its one-particle marginal and [two-particle distribution function](../../../../two-particle-distribution-function.md):

$$
f(z_1)=N\int D_N\,dz_2\cdots dz_N,\qquad f_2(z_1,z_2)=N(N-1)\int D_N\,dz_3\cdots dz_N.
$$

Thus $\int f\,dz=N$ and $\int f_2(z_1,z_2)\,dz_2=(N-1)f(z_1)$. For unit particle [mass](../../../../mass.md), $f$ also carries [mass density](../../../../density.md). These conventions explain why no extra factor $N-1$ occurs in the result.

Separate the [Hamiltonian](../../../../hamiltonian.md) as $H=H_1+H_{\mathrm{rest}}+H_{\mathrm{int}}$, where

$$
H_1=\frac12|\mathbf v_1|^2,\qquad H_{\mathrm{int}}=\sum_{j=2}^N\phi(|\mathbf x_1-\mathbf x_j|),
$$

and $H_{\mathrm{rest}}$ contains all terms involving only particles $2,\ldots,N$. The stated [Poisson bracket](../../../../poisson-bracket.md) gives [Hamilton's equations](../../../../hamilton-s-equations.md)

$$
\dot{\mathbf x}_i=\mathbf v_i,\qquad \dot{\mathbf v}_i=-\sum_{j\ne i}\nabla_{\mathbf x_i}\phi(|\mathbf x_i-\mathbf x_j|).
$$

Conservation of probability along the [Hamiltonian flow](../../../../hamiltonian-flow.md) gives the [Hamiltonian Liouville equation](../../../../hamiltonian-liouville-equation.md)

$$
\partial_tD_N+\sum_{i=1}^N\left[\mathbf v_i\cdot\nabla_{\mathbf x_i}D_N-\sum_{j\ne i}\nabla_{\mathbf x_i}\phi_{ij}\cdot\nabla_{\mathbf v_i}D_N\right]=0.
$$

Assume decay of the required [velocity moments](../../../../velocity-moment.md) and either decay or periodic [boundary conditions](../../../../boundary-condition.md) in position. Integrating over $z_2,\ldots,z_N$ eliminates the $H_{\mathrm{rest}}$ terms by [integration by parts](../../../../integration-by-parts.md). The terms in $H_{\mathrm{int}}$ differentiating an integrated [velocity](../../../../velocity.md) also vanish. Indistinguishability makes the remaining $N-1$ terms equal, so

$$
\begin{aligned}
\partial_tf+\mathbf v_1\cdot\nabla_{\mathbf x_1}f
&=N\sum_{j=2}^N\int\nabla_{\mathbf x_1}\phi_{1j}\cdot\nabla_{\mathbf v_1}D_N\,dz_2\cdots dz_N\\
&=\int dz_2\,\nabla_{\mathbf x_1}\phi_{12}\cdot\nabla_{\mathbf v_1}f_2.
\end{aligned}
$$

Relabeling the two particles gives the first [BBGKY hierarchy](../../../../bbgky-hierarchy.md) equation:

$$
\boxed{\partial_tf+\mathbf v\cdot\nabla_{\mathbf x}f=\int d^3x_\star\,d^3v_\star\,\nabla_{\mathbf v}f_2\cdot\nabla_{\mathbf x}\phi(|\mathbf x-\mathbf x_\star|).}
$$

This is exact for a differentiable [pair potential](../../../../pair-potential.md); no independent-particle closure has been made.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
