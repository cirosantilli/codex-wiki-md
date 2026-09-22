<h1 id="8/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

By hypothesis the [power series](../../../../../../power-series.md) converges at every positive real argument, so its [radius of convergence](../../../../../../radius-of-convergence.md) is infinite. Termwise [differentiation of a power series](../../../../../../termwise-differentiation-of-a-power-series.md) is therefore valid in a neighborhood of $s=1$. For $k\ge1$,

$$
G^{(k)}(s)=\sum_{j=k}^{\infty}
j(j-1)\cdots(j-k+1)p(j)s^{j-k}.
$$

At $s=1$, the right side is the [expectation](../../../../../../expected-value-split.md) of the [falling factorial](../../../../../../falling-factorial.md) of $X$:

$$
\boxed{G^{(k)}(1)=\mathbb E[X(X-1)\cdots(X-k+1)].}
$$

The special case $k=1$ gives

$$
\boxed{G'(1)=\mathbb E[X].}
$$

For $k=0$, take the empty product as $1$; the equality becomes $G(1)=1$. These are the [factorial moments](../../../../../../factorial-moment.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
