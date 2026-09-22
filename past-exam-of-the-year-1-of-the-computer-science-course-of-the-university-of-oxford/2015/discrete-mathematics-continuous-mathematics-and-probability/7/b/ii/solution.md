<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [absorbing states](../../../../../../absorbing-state.md) give $e_0=e_n=0$. Multiplying the [difference equation](../../../../../../difference-equation.md) in (i) by $3$ gives

$$
e_{k+1}-2e_k+e_{k-1}=-3.
$$

The second [finite difference](../../../../../../finite-difference-split.md) of $k^2$ is $2$, so a [particular solution](../../../../../../particular-solution.md) is $-3k^2/2$; the homogeneous solutions are $A+Bk$. Imposing the two [boundary conditions](../../../../../../boundary-condition.md) gives $A=0,B=3n/2$. Therefore

$$
\boxed{e_k=\frac32k(n-k),\qquad0\le k\le n.}
$$

Uniqueness follows because the difference of any two solutions has zero second [finite difference](../../../../../../finite-difference-split.md), hence is [affine function](../../../../../../affine-function.md), and vanishes at both endpoints. This is the [mean absorption time of a lazy symmetric random walk](../../../../../../mean-absorption-time-of-a-lazy-symmetric-random-walk.md) with holding probability $1/3$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
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
