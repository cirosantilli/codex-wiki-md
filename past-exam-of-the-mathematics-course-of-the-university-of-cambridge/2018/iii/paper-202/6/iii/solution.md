<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The limit is in [probability](../../../../../../probability.md), or more strongly in [uniform convergence on compacts in probability](../../../../../../uniform-convergence-on-compacts-in-probability.md); a pathwise limit for every [continuous local martingale](../../../../../../continuous-local-martingale.md) is not implicit. The original PDF uses $\lceil t2^n\rceil$, whereas the supplied TeX changes this to $\lfloor t2^n\rfloor$; both versions have the same limit by continuity.

Put $\delta=2^{-n}$ and $m=\lfloor t/\delta\rfloor$. For the completed intervals, the algebraic identity

$$
\sum_{i=1}^m\frac{Y_{i\delta}+Y_{(i-1)\delta}}2\,(X_{i\delta}-X_{(i-1)\delta})
=\sum_{i=1}^mY_{(i-1)\delta}\Delta_iX+\frac12\sum_{i=1}^m\Delta_iY\,\Delta_iX
$$

separates a left-point sum from a [quadratic covariation](../../../../../../quadratic-covariation.md) sum.

The results from [stochastic calculus](../../../../../../stochastic-calculus-split.md) used are these: predictable left-step approximations to a continuous [adapted](../../../../../../adapted-process.md) integrand converge in their [Itô integrals](../../../../../../ito-integral.md) in [uniform convergence on compacts in probability](../../../../../../uniform-convergence-on-compacts-in-probability.md); and products of increments of continuous [semimartingales](../../../../../../semimartingale.md) on deterministic [partitions of an interval](../../../../../../partition-of-an-interval.md) with vanishing mesh converge to their [quadratic covariation](../../../../../../quadratic-covariation.md) in the same sense. The first follows after localization from the [Itô isometry](../../../../../../ito-isometry.md) and the [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md), since the integrand approximations converge uniformly on compact intervals; the second is the deterministic-partition characterization of [quadratic covariation](../../../../../../quadratic-covariation.md).

Thus the two sums converge to $\int_0^tY_s\,dX_s$ and $\frac12\langle Y,X\rangle_t$. For the ceiling convention, at most one additional full interval extends past $t$; on $[0,T+1]$ its absolute contribution is at most $\sup_{s\leq T+1}|Y_s|$ times the modulus of continuity of $X$ at scale $\delta$, which tends to zero [almost surely](../../../../../../almost-sure-convergence.md). Therefore

$$
\boxed{\sum_{i=1}^{\lceil t2^n\rceil}\frac{Y_{i2^{-n}}+Y_{(i-1)2^{-n}}}{2}\,(X_{i2^{-n}}-X_{(i-1)2^{-n}})\xrightarrow[n\to\infty]{\mathbb P}\int_0^tY_s\circ dX_s.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
