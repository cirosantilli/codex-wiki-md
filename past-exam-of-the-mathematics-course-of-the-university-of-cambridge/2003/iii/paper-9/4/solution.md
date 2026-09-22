<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

First construct a [holomorphic function](../../../../../holomorphic-function.md) without requiring boundedness. Separate the finitely many zeros at zero into $z^m$, and enumerate the remaining prescribed zeros as $a_n$. Since $|a_n|\to1$, there is no interior accumulation point and every prescribed point has finite [multiplicity](../../../../../multiplicity-mathematics.md). Using the [Weierstrass elementary factors](../../../../../weierstrass-elementary-factor.md), set

$$
F(z)=z^m\prod_{n\ge1}E_n(z/a_n),\qquad
E_n(t)=(1-t)\exp\left(\sum_{k=1}^n\frac{t^k}{k}\right).
$$

For a compact disc $|z|\le r<1$, choose $q$ with $r<q<1$. Eventually $|z/a_n|\le q$. The [power series](../../../../../power-series.md) identity

$$
\log E_n(t)=-\sum_{k=n+1}^\infty\frac{t^k}{k},\qquad
|\log E_n(t)|\le\frac{q^{n+1}}{(n+1)(1-q)}
$$

gives an absolutely summable uniform bound. The [infinite product convergence from logarithmic tails](../../../../../infinite-product-convergence-from-logarithmic-tails.md) therefore makes the tail [holomorphic](../../../../../complex-differentiability-at-a-point.md) and nonvanishing on this compact set. The finitely many initial factors have exactly their prescribed zeros, with the prescribed [multiplicities](../../../../../multiplicity-mathematics.md). Hence $F$ has exactly the required zero sequence. This is a direct [canonical product construction for zeros escaping to the disk boundary](../../../../../canonical-product-construction-for-zeros-escaping-to-the-disk-boundary.md).

For a nonzero bounded [holomorphic function](../../../../../holomorphic-function.md), [Jensen's formula](../../../../../jensen-s-formula.md) bounds $\sum_n\log(1/|a_n|)$ after separating the zero at zero. Thus the [Blaschke condition](../../../../../blaschke-condition.md) is necessary; the [Blaschke product](../../../../../blaschke-product.md) construction makes it sufficient. Use the curvature-minus-one convention for [Hyperbolic distance in the Poincare disc](../../../../../hyperbolic-distance-in-the-poincare-disc.md):

$$
\rho(0,z)=\log\frac{1+|z|}{1-|z|},\qquad
e^{-\rho(0,z)}=\frac{1-|z|}{1+|z|}.
$$

The latter lies between $(1-|z|)/2$ and $1-|z|$. Consequently the precise bounded-function criterion is

$$
\boxed{\sum_n e^{-\rho(0,z_n)}<\infty.}
$$

This counts [multiplicities](../../../../../multiplicity-mathematics.md); the finitely many occurrences at zero cause no problem.

For the requested [hyperbolic zero estimate for a Blaschke product](../../../../../hyperbolic-zero-estimate-for-a-blaschke-product.md), the [pseudohyperbolic distance](../../../../../pseudohyperbolic-distance.md) identity is

$$
|b_a(w)|=\left|\frac{w-a}{1-\overline a w}\right|
=\tanh\frac{\rho(w,a)}2=\frac{1-t}{1+t},\qquad t=e^{-\rho(w,a)}.
$$

If $w$ is not a zero, $0<t<1$. The real function $L(t)=\log[(1+t)/(1-t)]-2t$ has $L(0)=0$ and $L'(t)=2t^2/(1-t^2)\ge0$, so $L(t)\ge0$. Thus $\log|b_a(w)|\le-2e^{-\rho(w,a)}$. Apply this to each factor, including factors at zero, and then pass from finite products to the [Blaschke product](../../../../../blaschke-product.md) by [locally uniform convergence](../../../../../locally-uniform-convergence.md):

$$
\boxed{|B(w)|\le\exp\left(-2\sum_n e^{-\rho(w,z_n)}\right).}
$$

At a zero of $B$ the left side is zero, so the inequality is immediate; the logarithmic calculation at $t=1$ is unnecessary. The unimodular constant contributes nothing. Away from the zeros the product is nonzero, so the same inequality also bounds the sum and shows it is finite there.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
