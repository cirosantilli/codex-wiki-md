<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the half-line [Fourier transform](../../../../../../fourier-transform.md) and finite-time boundary transforms

$$
\widehat q(k,t)=\int_0^\infty e^{-ikx}q(x,t)\,dx,\qquad G_j(k,t)=\int_0^t e^{ik^2s}g_j(s)\,ds,\quad g_j(t)=\partial_x^jq(0,t),\quad j=0,1.
$$

The half-line [Fourier transform](../../../../../../fourier-transform.md) is analytic for $\operatorname{Im}k<0$ under spatial decay. All spectral integrals below have their usual oscillatory, or vanishing Gaussian damping, interpretation until absolute convergence is established.

The [free Schrodinger equation](../../../../../../free-schrodinger-equation.md) has the local divergence identity

$$
\partial_t(e^{-ikx+ik^2t}q)=i\partial_x\left[e^{-ikx+ik^2t}(q_x+ikq)\right].
$$

Integrating in $x,t$ gives the [global relation for the half-line free Schrodinger equation](../../../../../../global-relation-for-the-half-line-free-schrodinger-equation.md)

$$
\boxed{e^{ik^2t}\widehat q(k,t)=\widehat q_0(k)+kG_0(k,t)-iG_1(k,t),\qquad\operatorname{Im}k\leq0.}
$$

Let $D_+=\{\operatorname{Re}k>0,\operatorname{Im}k>0\}$. Orient its boundary from $i\infty$ down to $0$, and then from $0$ to $+\infty$, so that $D_+$ lies on the left. [Fourier inversion](../../../../../../fourier-inversion-theorem.md) followed by [contour integration](../../../../../../contour-integration.md) in the second quadrant yields

$$
\boxed{q(x,t)=\frac1{2\pi}\int_{\mathbb R}e^{ikx-ik^2t}\widehat q_0(k)\,dk+\frac1{2\pi}\int_{\partial D_+}e^{ikx-ik^2t}\left[kG_0(k,t)-iG_1(k,t)\right]dk.}
$$

This is a complex spectral representation involving the initial trace and both boundary traces. The contour deformation works because each boundary-time integrand contains $e^{-ik^2(t-s)}$ with $s\leq t$, which decays in the second quadrant, as well as $e^{ikx}$ for $x>0$. This fixes both the quadrant and the orientation; changing either without changing the signs would produce an incorrect representation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
