<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**The assertion requires $p+q>0$.** As printed, it also includes $(p,q)=(0,0)$, where the nonzero constant function $1$ is closed but cannot be the [exterior derivative](../../../../../../exterior-derivative.md) of a negative-degree form. The zero constant is harmless; below we prove the intended positive-degree result.

Set $k=p+q>0$, let $\rho_t(z)=tz$, and let

$$
R=\sum_j\left(z_j\frac{\partial}{\partial z_j}+\bar z_j\frac{\partial}{\partial\bar z_j}\right).
$$

The [polydisc](../../../../../../polydisc.md) is preserved by these dilations. The [radial homotopy operator](../../../../../../radial-homotopy-operator.md) is

$$
\boxed{H\alpha=\int_0^1\rho_t^*(\iota_R\alpha)\,\frac{dt}{t}.}
$$

Here $\iota_R$ is the [interior product of a differential form](../../../../../../interior-product.md). For a smooth $k$-form, its pulled-back contraction is $O(t^k)$, so the integral and its coefficient derivatives converge at zero. The identity for a [pullback of a differential form](../../../../../../pullback-of-a-differential-form.md) along the radial flow and [Cartan's magic formula](../../../../../../cartan-s-magic-formula.md) give

$$
\frac{d}{dt}\rho_t^*\alpha=\frac1t\rho_t^*\mathcal L_R\alpha
=\frac1t\rho_t^*(d\iota_R\alpha+\iota_Rd\alpha).
$$

Integrating yields $dH\alpha+Hd\alpha=\alpha-\rho_0^*\alpha$. The final pullback vanishes in positive degree; since $d\alpha=0$, we have $dH\alpha=\alpha$.

Each $\rho_t$ is a [holomorphic map](../../../../../../holomorphic-map.md), so its [pullback of a differential form](../../../../../../pullback-of-a-differential-form.md) preserves bidegree. Contracting with the $(1,0)$ part of $R$ lowers $p$ by one, and contracting with its $(0,1)$ part lowers $q$ by one. Therefore the primitive has precisely the permitted types:

$$
\boxed{\beta=H\alpha\in\mathcal A^{p-1,q}(D)\oplus\mathcal A^{p,q-1}(D),\qquad d\beta=\alpha.}
$$

This is a type-preserving refinement of the [Poincaré lemma](../../../../../../poincare-lemma.md); when one index is zero, the corresponding negative-degree summand is simply absent.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
