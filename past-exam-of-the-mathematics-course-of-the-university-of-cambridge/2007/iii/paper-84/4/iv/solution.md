<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $N=\int_S n\,dS$ be the particle number per unit axial length, and consider the axially homogeneous equilibrium implicit in a cross-sectional description. Integrating the stationary [gain-loss Madelung equations](../../../../../../gain-loss-madelung-equations.md) over $S$ and applying the [divergence theorem](../../../../../../divergence-theorem.md) gives

$$
\oint_{\partial S}n\nabla_\perp\Phi\cdot\boldsymbol\nu\,dl
=\frac2\hbar\left(\gamma N-\Gamma\int_S n^2\,dS\right).
$$

The wall condition $n=0$ means the lateral [condensate number current](../../../../../../condensate-number-current.md) vanishes. This is also directly apparent from $\mathbf j=(\hbar/m)\operatorname{Im}(\Psi^*\nabla\Psi)$ for a regular Dirichlet wavefunction, without assigning a phase at its zeros. Consequently the [cylindrical pump-loss balance](../../../../../../cylindrical-pump-loss-balance.md) is

$$
\boxed{\int_S n^2\,dS=qN,\qquad q=\frac\gamma\Gamma}.
$$

Integrated particle creation equals integrated nonlinear loss; there is no assumption that $n=q$ pointwise. In fact the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives $N^2\le|S|\int_Sn^2=|S|qN$, so a nonzero equilibrium obeys $N\le q|S|$.

The axial condition is needed for a slice-by-slice statement. More generally, put $J(z)=\int_S n\partial_z\Phi\,dS$. Lateral no-flux and stationary density give

$$
J'(z)=\frac2\hbar\left[\gamma N(z)-\Gamma\int_S n^2\,dS\right],\qquad
\int_S n^2\,dS=\frac\gamma\Gamma N(z)-\frac\hbar{2\Gamma}J'(z).
$$

Thus the requested equality also holds whenever the integrated axial current is constant. If axially inhomogeneous equilibria with nonzero axial flux divergence are allowed, the lateral boundary condition alone proves this more general balance, rather than the stated equality at every cross-section.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
