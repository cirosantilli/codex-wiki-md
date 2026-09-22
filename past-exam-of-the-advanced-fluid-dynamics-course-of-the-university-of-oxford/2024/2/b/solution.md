<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $K_{ij}=\partial_j u_i$, $C_{ij}=\langle R_iR_j\rangle$, $\alpha=2H/\zeta$ and $D_R=2k_BT/\zeta$. The configuration equation of the [Hookean dumbbell model](../../../../hookean-dumbbell-model.md) becomes

$$
\partial_t\psi=-\nabla_{\mathbf R}\cdot[(K\mathbf R-\alpha\mathbf R)\psi]+D_R\nabla_{\mathbf R}^2\psi.
$$

Here the paper's $k$ denotes the [Boltzmann constant](../../../../boltzmann-constant.md) $k_B$. Integrating the [second moment](../../../../second-moment.md) equation against $R_iR_j$ and discarding boundary terms at infinite separation gives

$$
\dot C_{ij}=K_{i\ell}C_{\ell j}+K_{j\ell}C_{i\ell}-2\alpha C_{ij}+2D_R\delta_{ij}.
$$

For example the spring drift differentiates each factor $R_i,R_j$, while the [Laplacian](../../../../laplacian.md) gives $\nabla_{\mathbf R}^2(R_iR_j)=2\delta_{ij}$. The [Hookean dumbbell conformation equation](../../../../hookean-dumbbell-conformation-equation.md) is

$$
\boxed{\dot C-KC-CK^T=\frac{4k_BT}{\zeta}I-\frac{4H}{\zeta}C.}
$$

In the row-vector convention of $\mathbf R\cdot\nabla\mathbf u$, the displayed gradient tensor is $K^T$, giving exactly the transposes in the requested equation. The dimensionless [conformation tensor](../../../../conformation-tensor.md) $A=HC/(k_BT)$ consequently has [upper-convected derivative](../../../../upper-convected-derivative.md) $-(A-I)/\lambda$, with [polymer relaxation time](../../../../polymer-relaxation-time.md) $\lambda=\zeta/(4H)$. This normalization matters: the unscaled $C$ has equilibrium value $(k_BT/H)I$, rather than $I$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
