<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [b](../b.md)

The [polynomial](../../../../../../polynomial-split.md) factors as $p(x)=(3x-2)^2(3x+1)$, so $\alpha=2/3$ is a [multiple root](../../../../../../multiple-root.md) of multiplicity two. The [Newton root-finding iteration](../../../../../../newton-root-finding-iteration.md) is

$$
x_{k+1}=x_k-\frac{p(x_k)}{p'(x_k)},\qquad p'(x)=81x^2-54x.
$$

For $x\ne0,2/3$, cancelling a factor gives

$$
\boxed{g(x)=\frac{2x}{3}+\frac19+\frac{2}{27x}.}
$$

This expression extends continuously to $g(2/3)=2/3$. Let $I=[1/3,1]$. On this [closed interval](../../../../../../closed-real-interval.md),

$$
g'(x)=\frac23-\frac{2}{27x^2},\qquad 0\le g'(x)\le\frac{16}{27}<1.
$$

Thus $g$ is increasing, and

$$
g(I)=[g(1/3),g(1)]=[5/9,23/27]\subset I.
$$

By the [mean value theorem](../../../../../../mean-value-theorem.md), $|g(x)-g(y)|\le(16/27)|x-y|$ for all $x,y\in I$. The [contraction mapping theorem](../../../../../../contraction-mapping-theorem.md) states that a [contraction mapping](../../../../../../contraction-mapping.md) from a nonempty [complete metric space](../../../../../../complete-metric-space.md) into itself has a unique [fixed point](../../../../../../fixed-point.md), and every [fixed-point iteration](../../../../../../fixed-point-iteration.md) converges to it. The [closed interval](../../../../../../closed-real-interval.md) $I$ with ordinary [Euclidean distance](../../../../../../euclidean-distance.md) is complete, and $g(2/3)=2/3$, so

$$
\boxed{x_k\longrightarrow\frac23\quad\text{for every }x_0\in[1/3,1].}
$$

In fact $|x_k-2/3|\le(16/27)^k|x_0-2/3|$. The [Newton iteration at a multiple root](../../../../../../newton-iteration-at-a-multiple-root.md) here has [linear convergence](../../../../../../linear-convergence.md), since $g'(2/3)=1/2$. Thus **the convergence assertion is true for the simplified [fixed-point iteration](../../../../../../fixed-point-iteration.md)**, and for the usual [Newton root-finding iteration](../../../../../../newton-root-finding-iteration.md) that stops upon reaching an exact [root of a polynomial](../../../../../../root-of-a-polynomial.md). If one insists on applying the unsimplified quotient at every step, it is undefined for the allowed starting value $x_0=2/3$, since both $p$ and $p'$ vanish there; that literal version of an infinite [sequence](../../../../../../sequence.md) requires the stated stopping convention or continuous extension.

## ↑ Ancestors (12)

1. [b](../b.md)
2. [7](../../7.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
