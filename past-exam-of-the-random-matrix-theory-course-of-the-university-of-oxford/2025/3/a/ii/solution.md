<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The difference of the two [eigenvalues](../../../../../eigenvalue.md) is $2i\sin U$, hence $\Delta=\sin^2U$. Its [expectation](../../../../../expected-value-split.md) is

$$
\boxed{\mathbb E\Delta=\frac1{2\pi}\int_0^{2\pi}\sin^2u\,du=\frac12.}
$$

For $0\leq x\leq1$, put $\alpha=\arcsin\sqrt{x}\in[0,\pi/2]$. The set of angles satisfying $|\sin u|\leq\sqrt{x}$ consists of $[0,\alpha]$, $[\pi-\alpha,\pi+\alpha]$ and $[2\pi-\alpha,2\pi]$, of total length $4\alpha$. Thus the full [cumulative distribution function](../../../../../cumulative-distribution-function.md) is

$$
\boxed{F_\Delta(x)=
\begin{cases}
0,&x<0,\\
\dfrac2\pi\arcsin\sqrt{x},&0\leq x\leq1,\\
1,&x>1.
\end{cases}}
$$

Differentiating on $(0,1)$ gives the [probability density function](../../../../../probability-density-function.md)

$$
\boxed{f_\Delta(x)=\frac1{\pi\sqrt{x(1-x)}},\qquad0<x<1.}
$$

This is the [arcsine distribution](../../../../../arcsine-distribution.md), equivalently the [beta distribution](../../../../../beta-distribution.md) with both parameters $1/2$. It has no atoms at either endpoint.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the random matrix theory course of the University of Oxford](../../../../split.md)
6. [Random matrix theory course of the University of Oxford](../../../../../random-matrix-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
