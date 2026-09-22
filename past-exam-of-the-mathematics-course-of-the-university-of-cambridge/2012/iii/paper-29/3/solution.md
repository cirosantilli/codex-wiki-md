<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For $\operatorname{Re}s>1$, define the [Riemann zeta function](../../../../../riemann-zeta-function.md) by the absolutely convergent [Dirichlet series](../../../../../dirichlet-series.md)

$$
\zeta(s)=\sum_{n\geq1}n^{-s}=\prod_p(1-p^{-s})^{-1}.
$$

The [Euler product](../../../../../euler-product.md) follows from [unique prime factorization](../../../../../fundamental-theorem-of-arithmetic.md) and [absolute convergence](../../../../../absolute-convergence.md). The counting-function integral gives

$$
\zeta(s)=s\int_1^\infty\lfloor u\rfloor u^{-s-1}\,du
=\frac{s}{s-1}-s\int_1^\infty\{u\}u^{-s-1}\,du.
$$

Because the [fractional part](../../../../../fractional-part.md) is bounded, the last integral, and its derivatives with respect to $s$ on compact subsets, converge uniformly for $\operatorname{Re}s>0$. It is a [holomorphic function](../../../../../holomorphic-function.md) there. This proves the [Meromorphic continuation of the Riemann zeta function to the right half-plane](../../../../../meromorphic-continuation-of-the-riemann-zeta-function-to-the-right-half-plane.md), with a [simple pole](../../../../../simple-pole.md) at one of [residue](../../../../../residue.md) one and no other singularity in that half-plane.

The [Gamma function](../../../../../gamma-function.md) is

$$
\Gamma(z)=\int_0^\infty e^{-u}u^{z-1}\,du\qquad(\operatorname{Re}z>0).
$$

The [Gamma function recurrence](../../../../../gamma-function-recurrence.md) extends it meromorphically; its poles are at the nonpositive integers and it has no zeros. The [functional equation of the Riemann zeta function](../../../../../functional-equation-of-the-riemann-zeta-function.md) can be stated as

$$
\boxed{\pi^{-s/2}\Gamma(s/2)\zeta(s)
=\pi^{-(1-s)/2}\Gamma((1-s)/2)\zeta(1-s),}
$$

or, equivalently,

$$
\boxed{\zeta(s)=2^s\pi^{s-1}\sin(\pi s/2)\Gamma(1-s)\zeta(1-s).}
$$

These are identities of [meromorphic functions](../../../../../meromorphic-function.md); the second also extends the [Riemann zeta function](../../../../../riemann-zeta-function.md) to the remaining half-plane. The [critical strip](../../../../../critical-strip.md) is $0<\operatorname{Re}s<1$; its boundary lines will also be treated below, rather than included among possible exceptional zeros.

For $\operatorname{Re}s>1$, the absolutely convergent reciprocal [Euler product](../../../../../euler-product.md) gives $\zeta(s)\neq0$. For $\operatorname{Re}s<0$, the factors $2^s$, $\pi^{s-1}$, $\Gamma(1-s)$ and $\zeta(1-s)$ in the second [functional equation of the Riemann zeta function](../../../../../functional-equation-of-the-riemann-zeta-function.md) are finite and nonzero. Hence the only zeros there are the zeros of the sine factor:

$$
\boxed{s=-2,-4,-6,\ldots.}
$$

Each is simple. At zero, the sine zero cancels the pole of $\zeta(1-s)$; using its [residue](../../../../../residue.md) one gives $\zeta(0)=-1/2$, not zero. Nonvanishing on the rest of $\operatorname{Re}s=0$ follows from the boundary-line proof below and the [functional equation of the Riemann zeta function](../../../../../functional-equation-of-the-riemann-zeta-function.md). Together these facts prove that the [trivial zeros of the Riemann zeta function](../../../../../trivial-zero-of-the-riemann-zeta-function.md) are the only zeros outside the open [critical strip](../../../../../critical-strip.md).

Here is a [Jensen disk proof of the zeta zero-count bound](../../../../../jensen-disk-proof-of-the-zeta-zero-count-bound.md) which avoids any unproved left-half-plane growth estimate. Set $F(s)=(s-1)\zeta(s)$, a [holomorphic function](../../../../../holomorphic-function.md) throughout $\operatorname{Re}s>0$, including at one. The integral continuation formula gives

$$
|F(s)|\ll(|s|+1)^2\qquad(\operatorname{Re}s\geq1/4).
$$

For each integer $j$, apply [Jensen's formula](../../../../../jensen-s-formula.md) in the disk with centre $2+ij$, outer radius $R=7/4$ and inner radius $r=8/5$. The outer disk stays in $\operatorname{Re}s\geq1/4$, so its maximum modulus is $O((|j|+2)^2)$. At its centre,

$$
|\zeta(2+ij)|\geq\zeta(2)^{-1},
\qquad |F(2+ij)|\geq|1+ij|/\zeta(2),
$$

since $|1/\zeta(2+ij)|\leq\sum_n|\mu(n)|n^{-2}\leq\zeta(2)$. Therefore the number of zeros in its inner disk, counted with multiplicity, is at most

$$
\frac{\log\bigl(\max_{|s-(2+ij)|\leq R}|F(s)|/|F(2+ij)|\bigr)}{\log(R/r)}
\ll\log(|j|+2).
$$

The rectangle $1/2\leq\operatorname{Re}s\leq1$, $|\operatorname{Im}s-j|\leq1/2$ fits in the inner disk because its farthest point has distance $\sqrt{(3/2)^2+(1/2)^2}=\sqrt{5/2}<8/5$. Summing over $O(T)$ such disks counts $O(T\log T)$ zeros in the right half of the [critical strip](../../../../../critical-strip.md) up to height $T$. The first [functional equation of the Riemann zeta function](../../../../../functional-equation-of-the-riemann-zeta-function.md) bijects zeros, with multiplicities, in the left half with their reflections $s\mapsto1-s$ in the right half; its [Gamma function](../../../../../gamma-function.md) factors are finite and nonzero in the strip. Thus

$$
\boxed{\#\{\rho:\zeta(\rho)=0,\ 0<\operatorname{Re}\rho<1,\ |\operatorname{Im}\rho|\leq T\}\ll T\log T.}
$$

The pole of [zeta function](../../../../../riemann-zeta-function.md) at one does not count as a zero: $F(1)=1$.

Finally, for real $\sigma>1$ and $t\neq0$, the Euler-product logarithms and the nonnegative [trigonometric polynomial](../../../../../trigonometric-polynomial.md)

$$
3+4\cos\theta+\cos(2\theta)=2(1+\cos\theta)^2\geq0
$$

give the [three-four-one product proof of zeta boundary nonvanishing](../../../../../three-four-one-product-proof-of-zeta-boundary-nonvanishing.md):

$$
\log\bigl(\zeta(\sigma)^3|\zeta(\sigma+it)|^4|\zeta(\sigma+2it)|\bigr)
=\sum_{p,k\geq1}\frac{3+4\cos(kt\log p)+\cos(2kt\log p)}{kp^{k\sigma}}\geq0.
$$

If $\zeta(1+it)$ had a zero of order $a\geq1$, its factor would be $O((\sigma-1)^{4a})$ as $\sigma\downarrow1$. The real [zeta function](../../../../../riemann-zeta-function.md) factor has pole order three, and the factor at $1+2it$ stays bounded because $t\neq0$. The product would tend to zero as $O((\sigma-1)^{4a-3})$, contradicting that it is at least one. Therefore

$$
\boxed{\zeta(1+it)\neq0\qquad(t\neq0).}
$$

At $t=0$ there is a pole, not a zero. Applying the sine-form [functional equation of the Riemann zeta function](../../../../../functional-equation-of-the-riemann-zeta-function.md) at $s=it\neq0$ now proves nonvanishing on the remaining imaginary axis, completing the earlier assertion about all zeros outside the [critical strip](../../../../../critical-strip.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
