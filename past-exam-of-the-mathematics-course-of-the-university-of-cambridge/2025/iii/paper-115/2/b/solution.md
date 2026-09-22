<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The metric on covectors is induced by the inverse matrix $g^{-1}$, and on $p$-forms by the determinant pairing

$$
\langle\alpha_1\wedge\cdots\wedge\alpha_p,
\beta_1\wedge\cdots\wedge\beta_p\rangle
=\det(\langle\alpha_i,\beta_j\rangle).
$$

The [Riemannian volume form](../../../../../../riemannian-volume-form.md) is the unique positive top form taking value one on every oriented orthonormal frame. The [Hodge star operator](../../../../../../hodge-star-operator.md) is uniquely determined by

$$
\beta\wedge *\alpha=\langle\beta,\alpha\rangle\omega_g.
$$

Nondegeneracy of the wedge pairing proves existence and uniqueness pointwise, and the smooth metric dependence makes $*$ a well-defined smooth bundle map.

On compactly supported forms, [Stokes theorem](../../../../../../stokes-theorem.md) and the graded Leibniz rule give

$$
\delta|_{\Omega^p}=(-1)^{m(p+1)+1}*d*,
$$

where $m=\dim M$; this is the formal $L^2$ adjoint of $d$. The Hodge [Laplace-Beltrami operator](../../../../../../laplace-beltrami-operator.md) is

$$
\Delta=d\delta+\delta d.
$$

For $g_f=e^{2f}g$, the covector metric scales by $e^{-2f}$, the $p$-form metric by $e^{-2pf}$, and the volume form by $e^{mf}$. Therefore

$$
*_f\alpha=e^{(m-2p)f}*\alpha.
$$

If $f$ is constant, the two star factors in the codifferential contribute $e^{-2f}$, so $\delta_f=e^{-2f}\delta$. Since $d$ is metric-independent,

$$
\boxed{\Delta_f\alpha=e^{-2f}\Delta\alpha.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
