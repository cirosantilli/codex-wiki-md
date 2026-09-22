<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**There is no proof of the printed assertion: it is false for the stated [expectations](../../../../../expected-value-split.md).** The original explicitly defines $x_j$ as the expected remaining count, so replacing it by a deterministic upper envelope changes the problem.[Printed p. 2, definition preceding Question 2(b), and Question 2(b)](../../../../../probability-and-computing-examination-paper-by-the-university-of-oxford-2015.md)

Let $B_j$ be the actual count after $j$ rounds and $x_j=\mathbb E B_j$. The [union bound](../../../../../boole-s-inequality.md) gives the valid conditional estimate

$$
\mathbb E[B_{j+1}\mid B_j=b]
\leq\frac{b(b-1)}n.
$$

By the [law of total expectation](../../../../../law-of-total-expectation.md), the resulting unconditional bound is

$$
\boxed{x_{j+1}\leq\frac{\mathbb E[B_j(B_j-1)]}{n}
=\frac{x_j^2-x_j+\operatorname{Var}(B_j)}n.}
$$

Discarding the [variance](../../../../../variance-split.md) term is an [expectation closure error for a nonlinear recurrence](../../../../../expectation-closure-error-for-a-nonlinear-recurrence.md). In particular, [Jensen's inequality](../../../../../jensen-s-inequality.md) says $\mathbb E B_j^2\geq x_j^2$, which cannot justify the requested upper bound.

For an exact [counterexample](../../../../../counterexample.md), start with two balls and two bins. A round serves both balls if they land separately and serves neither if they collide. Each outcome has [probability](../../../../../probability.md) $1/2$, independently in successive rounds while both balls remain. Consequently

$$
\mathbb P(B_j=2)=2^{-j},\qquad
\boxed{x_j=2^{1-j}.}
$$

At $j=2$, the requested inequality would say $x_3\leq x_2^2/2$, but

$$
\boxed{x_3=\frac14>\frac{(1/2)^2}{2}=\frac18.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Probability and computing](../../../probability-and-computing-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
