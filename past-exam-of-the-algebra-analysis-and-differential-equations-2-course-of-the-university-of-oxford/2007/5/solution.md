<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a [holomorphic function](../../../holomorphic-function-split.md) on $|z-a|<R$, the complex [Taylor theorem](../../../taylor-s-theorem.md) states

$$
f(z)=\sum_{n=0}^{\infty}\frac{f^{(n)}(a)}{n!}(z-a)^n\qquad(|z-a|<R),
$$

with uniform convergence on each smaller closed [disc](../../../topological-disc.md). Here is a proof. Choose $r<\rho<R$. For $|z-a|\le r$ and $|\zeta-a|=\rho$, the [geometric series](../../../geometric-series.md)

$$
\frac1{\zeta-z}=\sum_{n=0}^{\infty}\frac{(z-a)^n}{(\zeta-a)^{n+1}}
$$

converges uniformly. Substitute it into [Cauchy integral formula](../../../cauchy-integral-formula.md) and integrate term by term to get

$$
f(z)=\sum_{n=0}^{\infty}c_n(z-a)^n,\qquad
c_n=\frac1{2\pi i}\int_{|\zeta-a|=\rho}\frac{f(\zeta)}{(\zeta-a)^{n+1}}\,d\zeta.
$$

If $M_\rho=\max_{|\zeta-a|=\rho}|f(\zeta)|$, then $|c_n|\le M_\rho\rho^{-n}$. These bounds justify differentiating the [power series](../../../power-series.md) any fixed number of times on a smaller closed [disc](../../../topological-disc.md), by comparison with convergent differentiated [geometric series](../../../geometric-series.md). Evaluation at $a$ gives $f^{(n)}(a)=n!c_n$. Since every $|z-a|<R$ belongs to some such smaller [disc](../../../topological-disc.md), the formula holds throughout the stated [domain](../../../domain-mathematical-analysis.md).

The [identity theorem](../../../identity-theorem.md) says that two [holomorphic functions](../../../holomorphic-function-split.md) on a connected open subset of $\mathbb C$ are equal everywhere if their equality set has an accumulation point in that subset. Equivalently, a [holomorphic function](../../../holomorphic-function-split.md) with an interior accumulation point of zeros is identically zero there.

The proposed [Taylor coefficients](../../../taylor-coefficient.md) at $i$, including the specified value for $n=0$, give

$$
\sum_{n=0}^{\infty}\frac{(-1)^n(z-i)^n}{i^{n+1}}
=\frac{1/i}{1+(z-i)/i}=\frac1z\qquad(|z-i|<1).
$$

The function $1/z$ is [holomorphic](../../../holomorphic-function-split.md) on $\mathbb C\setminus\{0\}$ and has exactly the given [derivatives](../../../derivative.md), so it supplies existence. Any other admissible [holomorphic function](../../../holomorphic-function-split.md) has the same [Taylor series](../../../taylor-series.md) on $|z-i|<1$. The punctured plane is connected, so the [identity theorem](../../../identity-theorem.md) gives uniqueness:

$$
\boxed{f(z)=\frac1z\quad(z\ne0).}
$$

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2007](../../2007-split.md)
3. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations II course of the University of Oxford](../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
