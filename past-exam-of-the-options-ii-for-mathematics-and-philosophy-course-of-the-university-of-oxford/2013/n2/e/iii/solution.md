<h1 id="n2/e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $g(s)=G_T(s)$. For $0<s<1$, differentiate the power-series identity from part (ii):

$$
g'(s)=e^{\lambda(g(s)-1)}+s\lambda e^{\lambda(g(s)-1)}g'(s).
$$

Because $g(s)\leq1$ and $\lambda<1$, its denominator is positive. Using $g(s)=s e^{\lambda(g(s)-1)}$ gives

$$
g'(s)=\frac{g(s)/s}{1-\lambda g(s)}.
$$

As $s\uparrow1$, almost-sure finiteness and bounded convergence give $g(s)\to1$. On the other hand, monotone convergence in $g'(s)=\sum_{k\geq1}k\mathbb P(T=k)s^{k-1}$ gives $g'(s)\to\mathbb ET$, initially allowing infinity. The displayed formula makes this limit finite and proves

$$
\boxed{\mathbb E[T]=\frac1{1-\lambda}.}
$$

This establishes finiteness rather than assuming it when rearranging an expectation equation. It is the subcritical branching-process total-progeny mean.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [E](../../e.md)
3. [N2](../../../n2.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the options II for mathematics and philosophy course of the University of Oxford](../../../../split.md)
6. [Options II for mathematics and philosophy course of the University of Oxford](../../../../../options-ii-for-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and philosophy course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
8. [Mathematics and philosophy course of the University of Oxford](../../../../../mathematics-and-philosophy-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
