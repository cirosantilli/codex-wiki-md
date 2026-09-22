<h1 id="9/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Part (a) gives $\mathbb P(X\in\mathbb Z)=0$. Therefore the [ceiling function](../../../../../../ceiling-function.md) and [floor function](../../../../../../floor-function.md) satisfy $\lceil X\rceil=\lfloor X\rfloor+1$ almost surely. Both are integrable, since $0\le\lfloor X\rfloor\le X$ and $\lceil X\rceil\le X+1$. Thus **$\mathbb E[\lceil X\rceil]=\zeta(t-1)+1$**.

Now take expectations in $\lfloor X\rfloor\le X\le\lceil X\rceil$:

$$
\zeta(t-1)\le\frac{t-1}{t-2}\le\zeta(t-1)+1.
$$

Writing $s=t-1$, which ranges over every $s>1$, and rearranging yields

$$
\boxed{\frac1{s-1}\le\zeta(s)\le\frac{s}{s-1}\qquad(s>1).}
$$

These are the [zeta bounds from rounded Pareto variables](../../../../../../zeta-bounds-from-rounded-pareto-variables.md): rounding below and above converts one elementary [expected value](../../../../../../expected-value-split.md) into bounds on an infinite [series](../../../../../../series-mathematics.md).

## ↑ Ancestors (13)

1. [V](../v.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Discrete mathematics, probability and continuous mathematics](../../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
