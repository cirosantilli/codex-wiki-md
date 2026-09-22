<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $y_1=(1-x)^{-1}$, the [derivatives](../../../../../../derivative.md) are $y_1'=(1-x)^{-2}$ and $y_1''=2(1-x)^{-3}$. Consequently the left-hand side of the [ordinary differential equation](../../../../../../ordinary-differential-equation.md) is

$$
\frac{2}{1-x}-\frac{4}{1-x}+\frac{2}{1-x}=0
$$

where $x\ne1$.

Use [reduction of order](../../../../../../reduction-of-order.md), writing $y=u/(1-x)$. A direct application of the [product rule](../../../../../../product-rule.md) gives

$$
(1-x)^2y''-4(1-x)y'+2y=(1-x)u''-2u'.
$$

For $v=u'$ the resulting [first-order ordinary differential equation](../../../../../../first-order-ordinary-differential-equation.md) is $v'/v=2/(1-x)$ whenever $v\ne0$. [Integration](../../../../../../integral-split.md) yields $v=C(1-x)^{-2}$ and $u=A+B/(1-x)$; the case $v=0$ is already included. Hence

$$
\boxed{y(x)=\frac{A}{1-x}+\frac{B}{(1-x)^2}}
$$

on either interval $x<1$ or $x>1$. The two displayed [solutions of a differential equation](../../../../../../solution-of-a-differential-equation.md) are [linearly independent](../../../../../../linear-independence.md), so they span the [solution space of a homogeneous linear differential equation](../../../../../../solution-space-of-a-homogeneous-linear-differential-equation.md) on either interval. The point $x=1$ is a [singular point of a differential equation](../../../../../../singular-point-of-a-differential-equation.md) and cannot be crossed by a nonzero member of this family that remains finite there.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Calculus, probability, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../../calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
5. [2003](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
