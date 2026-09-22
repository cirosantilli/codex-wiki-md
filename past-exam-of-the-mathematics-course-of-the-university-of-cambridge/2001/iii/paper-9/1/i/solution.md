<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We use the complete [hyperbolic metric](../../../../../../hyperbolic-metric.md) of curvature $-1$; on the [unit disc](../../../../../../unit-disc.md) its length element is $2|dz|/(1-|z|^2)$. This normalization matters in the exponential summability criterion. A nonzero bounded [holomorphic function](../../../../../../holomorphic-function.md) on the entire plane is constant by [Liouville's theorem](../../../../../../liouville-theorem.md), so the prescribed infinite zero set forces $\Omega\ne\mathbb C$. The [Riemann mapping theorem](../../../../../../riemann-mapping-theorem.md) supplies a [biholomorphism](../../../../../../biholomorphism.md) $\phi:\Omega\to\mathbb D$, and transports the disk [hyperbolic metric](../../../../../../hyperbolic-metric.md) to $\Omega$.

Fix $w\in\Omega$ and choose $\phi(w)=0$. Put $a_n=\phi(z_n)$ and $F=f\circ\phi^{-1}$. First suppose $F(0)\ne0$. For radii avoiding its zeros, [Jensen's formula](../../../../../../jensen-s-formula.md) gives

$$
\sum_{|a_n|<r}\log\frac r{|a_n|}\le\log\|F\|_\infty-\log|F(0)|.
$$

The [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) as $r\uparrow1$ gives $\sum_n-\log|a_n|<\infty$, hence $\sum_n(1-|a_n|)<\infty$. If $F$ has a zero at zero, factor off its finite order first; the resulting [holomorphic function](../../../../../../holomorphic-function.md) is still bounded, since division by that power is bounded away from zero and extends near zero. Thus the [Blaschke condition](../../../../../../blaschke-condition.md) holds in either case, with the possible origin zero treated as one additional finite term.

The [Hyperbolic distance in the Poincare disc](../../../../../../hyperbolic-distance-in-the-poincare-disc.md) satisfies

$$
\rho(w,z_n)=\log\frac{1+|a_n|}{1-|a_n|},\qquad e^{-\rho(w,z_n)}=\frac{1-|a_n|}{1+|a_n|}\le1-|a_n|.
$$

Consequently **the exponential distances are summable**. This holds for every basepoint: the [triangle inequality](../../../../../../triangle-inequality.md) bounds the ratio of $e^{-\rho(w,z_n)}$ and $e^{-\rho(w_0,z_n)}$ between $e^{-\rho(w,w_0)}$ and $e^{\rho(w,w_0)}$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
