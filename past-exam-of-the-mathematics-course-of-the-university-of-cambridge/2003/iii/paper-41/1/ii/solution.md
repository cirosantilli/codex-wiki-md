<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [Probabilists' Hermite polynomials](../../../../../../probabilists-hermite-polynomial.md), rather than the differently scaled physicists' convention:

$$
H_r(x)=(-1)^re^{x^2/2}\frac{d^r}{dx^r}e^{-x^2/2}.
$$

Thus $H_2=x^2-1$, $H_3=x^3-3x$, and $H_5=x^5-10x^3+15x$. The [cumulant-generating function](../../../../../../cumulant-generating-function.md) of an exponential variable of mean $\theta$ is $-\log(1-\theta t)$ near zero, so its $r$th [cumulant](../../../../../../cumulant.md) is $(r-1)!\theta^r$. Hence the standardized third and fourth cumulants are $\rho_3=2$ and $\rho_4=6$; the fourth is a cumulant, not the fourth raw central moment.

Write $F_n$ for the [cumulative distribution function](../../../../../../cumulative-distribution-function.md) of the pivot in part (i). Its [Edgeworth expansion](../../../../../../edgeworth-series.md), valid here because the exponential law is smooth, nonlattice and has exponential moments, is

$$
F_n(t)=\Phi(t)-\phi(t)\left[\frac{H_2(t)}{3\sqrt n}+\frac{H_3(t)}{4n}+\frac{H_5(t)}{18n}\right]+O(n^{-3/2})
$$

at the fixed endpoints $t=\pm z$. The coverage is exactly $F_n(z)-F_n(-z)$. Since $H_2$ and $\phi$ are even, the $n^{-1/2}$ terms cancel; the two odd Hermite terms double. Consequently the [symmetric Edgeworth coverage cancellation](../../../../../../symmetric-edgeworth-coverage-cancellation.md) gives

$$
\boxed{\mathbb P_\theta(\theta\text{ lies in the interval})=1-\alpha-\frac{\phi(z)}n\left[\frac12H_3(z)+\frac19H_5(z)\right]+O(n^{-3/2}).}
$$

In particular its [coverage probability](../../../../../../coverage-probability.md) error is $\boxed{O(n^{-1})}$. This is a fixed-confidence-level expansion; it is not a uniform statement for normal cutoffs increasing with $n$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
