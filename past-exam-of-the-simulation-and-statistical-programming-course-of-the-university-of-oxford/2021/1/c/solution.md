<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An [importance weight](../../../../importance-weight.md) has [expected value](../../../../expected-value-split.md) $\mathbb E_q[w(Z)]=\int p(z)\,dz=1$. From the ratio in (a),

$$
\mathbb E_q[w(Z)^2]
=s^d\prod_{j=1}^d\mathbb E_{Z_j\sim N(0,s)}\!\left[e^{-(1-s^{-1})Z_j^2}\right].
$$

The supplied [normal distribution](../../../../normal-distribution.md) transform applies with quadratic coefficient $-(1-s^{-1})$, giving each factor $(2s-1)^{-1/2}$. Thus

$$
\boxed{\operatorname{Var}_q(w(Z))=\left(\frac{s}{\sqrt{2s-1}}\right)^d-1.}
$$

For $s>1$, the base $A:=s/\sqrt{2s-1}$ exceeds one because $s^2-(2s-1)=(s-1)^2>0$: [importance weight](../../../../importance-weight.md) [variance](../../../../variance-split.md) increases exponentially with dimension. For $s=1$, the [importance weight](../../../../importance-weight.md) is identically one and its [variance](../../../../variance-split.md) is zero. This calculation concerns the [importance weight](../../../../importance-weight.md), rather than the weighted integrand.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../split.md)
5. [Simulation and statistical programming course of the University of Oxford](../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
