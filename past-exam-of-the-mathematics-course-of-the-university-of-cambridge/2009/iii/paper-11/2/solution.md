<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Zeros are counted with their prescribed finite multiplicities, and the function is not identically zero. The criterion for [zero sets in the unit disc](../../../../../zero-sets-in-the-unit-disc.md) is **local finiteness: no point of the disc is an accumulation point of the zero sequence, and no point has infinite [multiplicity](../../../../../multiplicity-mathematics.md)**. Necessity follows from the [identity theorem for holomorphic functions](../../../../../identity-theorem.md). For sufficiency, factor a finite number of zeros at zero as $z^m$. For an infinite sequence of remaining zeros $a_n$, local finiteness implies $|a_n|\to1$. With [Weierstrass elementary factors](../../../../../weierstrass-elementary-factor.md)

$$
E_n(t)=(1-t)\exp\left(\sum_{j=1}^n\frac{t^j}{j}\right),
$$

use $f(z)=z^m\prod_nE_n(z/a_n)$. On each [compact](../../../../../compact-space.md) subdisc, eventually $|z/a_n|\le q<1$ and the logarithm of the tail factor is $-\sum_{j>n}(z/a_n)^j/j$, bounded in modulus by $q^{n+1}/((n+1)(1-q))$. These bounds are summable, so [infinite product convergence from logarithmic tails](../../../../../infinite-product-convergence-from-logarithmic-tails.md) gives [locally uniform convergence](../../../../../locally-uniform-convergence.md) and nonvanishing away from the listed zeros. Its finite initial factors give exactly their multiplicities. For a finite sequence an ordinary [polynomial](../../../../../polynomial-split.md) suffices.

Use the curvature-minus-one [hyperbolic metric](../../../../../hyperbolic-metric.md), with length element $2|dz|/(1-|z|^2)$. Integrating radially gives

$$
\rho(0,a)=\log\frac{1+|a|}{1-|a|},\qquad
\frac12(1-|a|)\le e^{-\rho(0,a)}=\frac{1-|a|}{1+|a|}\le1-|a|.
$$

Therefore the printed sum condition is equivalent to the [Blaschke condition](../../../../../blaschke-condition.md) $\sum_n(1-|a_n|)<\infty$.

To prove necessity for bounded $f$, first suppose $f(0)\ne0$ and choose a radius $r<1$ with no zero on its circle. Remove the finitely many factors $(z-a_n)$ for $|a_n|<r$. The logarithm of the modulus of the remaining zero-free function is [harmonic](../../../../../harmonic-function.md) on the closed disc. Its [mean value property](../../../../../mean-value-property-for-harmonic-functions.md), together with the mean of $\log|re^{i\theta}-a|$ being $\log r$ for $|a|<r$ (expand the logarithm in powers of $a/(re^{i\theta})$), proves [Jensen's formula](../../../../../jensen-s-formula.md)

$$
\sum_{|a_n|<r}\log\frac r{|a_n|}
=\frac1{2\pi}\int_0^{2\pi}\log|f(re^{i\theta})|\,d\theta-\log|f(0)|
\le\log\|f\|_\infty-\log|f(0)|.
$$

Let $r\uparrow1$ through such radii. Each summand increases to $-\log|a_n|$, and $-\log t\ge1-t$ for $0<t\le1$ by integration of $1/t\ge1$. Consequently $\sum_n(1-|a_n|)<\infty$. If $f$ has order $m$ at zero, apply the argument to $f/z^m$, which is still bounded: outside $|z|=1/2$ it is bounded by $2^m\|f\|_\infty$, and inside use the [maximum modulus principle](../../../../../maximum-modulus-principle.md). Add the finite contribution of the zeros at zero.

For sufficiency use a [Blaschke product](../../../../../blaschke-product.md). For $a\ne0$ its normalized [Blaschke factor](../../../../../blaschke-factor.md) is

$$
b_a(z)=\frac{|a|}{a}\frac{a-z}{1-\overline az},\qquad
1-b_a(z)=(1-|a|)\frac{1+(|a|/a)z}{1-\overline az}.
$$

On $|z|\le R<1$, $|1-b_a(z)|\le(1-|a|)(1+R)/(1-R)$. The [Blaschke condition](../../../../../blaschke-condition.md) thus makes the product converge locally uniformly; outside the specified zeros, the tail logarithms converge absolutely and the product is nonzero. Each factor has modulus at most one in the disc, so the limit is bounded by one. A factor $z^m$ supplies any finite [multiplicity](../../../../../multiplicity-mathematics.md) at zero. This proves

$$
\boxed{\text{A nonzero bounded holomorphic function with exactly these zeros exists}
\iff\sum_ne^{-\rho(0,a_n)}<\infty.}
$$

For the elementary inequality, put $H(t)=\log((1+t)/(1-t))-2t$. Then $H(0)=0$ and

$$
H'(t)=\frac2{1-t^2}-2=\frac{2t^2}{1-t^2}\ge0,
$$

so $\boxed{\log((1+t)/(1-t))\ge2t}$ for $0\le t<1$.

For any point $w$ not among the zeros, the [pseudohyperbolic distance](../../../../../pseudohyperbolic-distance.md) formula gives

$$
|b_a(w)|=\left|\frac{w-a}{1-\overline aw}\right|
=\tanh\frac{\rho(w,a)}2=\frac{1-e^{-\rho(w,a)}}{1+e^{-\rho(w,a)}}.
$$

Apply the proved inequality with $t=e^{-\rho(w,a)}$ to obtain $\log|b_a(w)|\le-2e^{-\rho(w,a)}$. Sum over finite products and pass to the limit, including factors at zero. This gives

$$
\boxed{|B(w)|\le\exp\left(-2\sum_ne^{-\rho(w,a_n)}\right).}
$$

The sum is finite: the [triangle inequality](../../../../../triangle-inequality.md) gives $e^{-\rho(w,a_n)}\le e^{\rho(0,w)}e^{-\rho(0,a_n)}$. If $w$ is itself a zero, $B(w)=0$ and the same bound is immediate, so no substitution at the excluded value $t=1$ is needed. A unimodular constant in $B$ has no effect.

If “zeros at the points” is interpreted as a set without assigned multiplicities, first delete repeated entries throughout. Otherwise infinitely repeating a single zero would invalidate the claimed necessity of the series condition; the standard zero-sequence convention counts multiplicities.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
