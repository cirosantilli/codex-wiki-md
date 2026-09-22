<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $f(x)=-\sum_i\log(\alpha_i+x_i)$. The feasible [probability simplex](../../../../../../probability-simplex.md) is a nonempty [compact convex set](../../../../../../compact-convex-set.md), so the [extreme value theorem](../../../../../../extreme-value-theorem.md) guarantees a minimizer. Its [Hessian matrix](../../../../../../hessian-matrix.md) is diagonal with positive entries $(\alpha_i+x_i)^{-2}$, making $f$ a [strictly convex function](../../../../../../strictly-convex-function.md). Hence **the minimizer is unique**.

Use the [Lagrange multipliers](../../../../../../lagrange-multiplier.md) $\lambda$ for the sum constraint and $\nu_i\geq0$ for $-x_i\leq0$. The [Lagrangian](../../../../../../lagrangian.md) is

$$
L=f(x)+\lambda\left(\sum_i x_i-1\right)-\sum_i\nu_i x_i.
$$

The [KKT conditions](../../../../../../karush-kuhn-tucker-conditions.md) are

$$
-\frac1{\alpha_i+x_i}+\lambda-\nu_i=0,\qquad
x_i\geq0,\quad \nu_i\geq0,\quad \nu_i x_i=0,\quad \sum_i x_i=1.
$$

A strictly positive feasible allocation exists, so the [Slater condition](../../../../../../slater-s-condition.md) holds. These conditions are necessary and sufficient for this [convex optimization](../../../../../../convex-optimization-split.md). At least one coordinate is positive, giving $\lambda>0$. Put $\tau=1/\lambda$. For a positive coordinate, [complementary slackness](../../../../../../complementary-slackness.md) gives $\alpha_i+x_i=\tau$. At a zero coordinate, stationarity gives $\nu_i=1/\tau-1/\alpha_i\geq0$, or $\alpha_i\geq\tau$. Thus

$$
\boxed{x_i^*=(\tau-\alpha_i)_+,\qquad
\sum_i(\tau-\alpha_i)_+=1.}
$$

Here $(u)_+=\max(u,0)$. This [logarithmic water filling](../../../../../../logarithmic-water-filling.md) raises the smaller baseline values to a common level. The scalar left side is a [continuous function](../../../../../../continuous-function.md) and strictly increasing above $\min_i\alpha_i$, starts at zero, and tends to infinity, so exactly one $\tau$ solves it. One can find it by [interval bisection](../../../../../../interval-bisection.md), or sort the baseline values increasingly and find an index $k$ for which

$$
\tau=\frac{1+\sum_{i=1}^k\alpha_{(i)}}k,
\qquad \alpha_{(k)}<\tau\leq\alpha_{(k+1)},
$$

using $\alpha_{(n+1)}=+\infty$. Equality at the next baseline simply gives a zero allocation. Sorting and a running sum implement the [water-filling algorithm](../../../../../../water-filling-algorithm.md) in $O(n\log n)$ time.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
