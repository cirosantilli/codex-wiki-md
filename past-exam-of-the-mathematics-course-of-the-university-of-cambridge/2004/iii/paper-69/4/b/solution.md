<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [zero-boundary Sobolev space](../../../../../../zero-boundary-sobolev-space.md) $V=H_0^1(0,1)$ with $\|v\|_V=\|v'\|_{L^2}$. The [Poincaré inequality](../../../../../../poincare-inequality.md) $\|v\|_{L^2}\le\pi^{-1}\|v'\|_{L^2}$ makes this a complete [Hilbert space](../../../../../../hilbert-space-split.md) norm. The [weak formulation](../../../../../../weak-formulation.md) is

$$
a(u,v)=\int_0^1[p(x)u'(x)v'(x)+q(x)u(x)v(x)]\,dx=\ell(v),\qquad\ell(v)=\int_0^1f(x)v(x)\,dx.
$$

Assume $p,q$ are measurable and satisfy the supplied bounds almost everywhere. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and [Poincaré inequality](../../../../../../poincare-inequality.md) give

$$
|a(u,v)|\le\left(p_1+\frac{q_1}{\pi^2}\right)\|u'\|_{L^2}\|v'\|_{L^2}.
$$

Because $p\ge p_0>0$ and $q\ge0$,

$$
a(v,v)=\int_0^1[p(v')^2+qv^2]\,dx\ge p_0\|v'\|_{L^2}^2.
$$

This is the [coercive variable-coefficient Dirichlet form](../../../../../../coercive-variable-coefficient-dirichlet-form.md). If $f\in L^2(0,1)$, then $|\ell(v)|\le\pi^{-1}\|f\|_{L^2}\|v\|_V$; more generally one may assume $f\in H^{-1}(0,1)=V'$. Some such source regularity is necessary to invoke the theorem. All hypotheses of the [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) now hold, with **coercivity constant $p_0$ and boundedness constant $p_1+q_1/\pi^2$**, giving the unique [weak solution](../../../../../../weak-solution.md) and every conforming [Galerkin method](../../../../../../galerkin-method.md) approximation. This argument does not require a pointwise derivative of $p$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
