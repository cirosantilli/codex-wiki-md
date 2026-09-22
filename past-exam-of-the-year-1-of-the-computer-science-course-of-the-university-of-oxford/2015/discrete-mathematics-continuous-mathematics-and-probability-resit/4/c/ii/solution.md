<h1 id="4/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The endpoint [boundary conditions](../../../../../../boundary-condition.md) are

$$
\boxed{y_0=1,\qquad y_N=5.}
$$

The [finite difference](../../../../../../finite-difference-split.md) equation can be written $y_{n+1}-2y_n+y_{n-1}=2h^2$. Set $d_n=y_n-y_{n-1}$. Then $d_{n+1}-d_n=2h^2$, so $d_n=d_1+2h^2(n-1)$. Summing from $1$ to $n$ gives

$$
y_n=1+nd_1+h^2n(n-1).
$$

Using $y_N=5$ and $h=2/N$ yields $Nd_1=4-h^2N(N-1)=4/N$, hence $d_1=4/N^2=h^2$. Therefore

$$
\boxed{y_n=1+h^2n^2=1+\left(\frac{2n}{N}\right)^2=y(x_n),\qquad 0\leq n\leq N.}
$$

This also covers $N=1$, where there are no interior equations. Uniqueness follows because the difference of two solutions has zero second [finite difference](../../../../../../finite-difference-split.md), hence is linear in $n$, and vanishes at both endpoints. This is an [exact finite difference solution for constant second derivative](../../../../../../exact-finite-difference-solution-for-constant-second-derivative.md): the method is exact at the nodes here because the centered second [finite difference](../../../../../../finite-difference-split.md) differentiates this quadratic [polynomial](../../../../../../polynomial-split.md) exactly.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Discrete mathematics, continuous mathematics, and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
