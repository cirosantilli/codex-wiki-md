<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $M_n=\max_{1\leq i\leq n}X_i$. For $0<s<1/c$, the exponential of a maximum is bounded by a sum, giving

$$
e^{sM_n}\leq\sum_{i=1}^n e^{sX_i},\qquad
\mathbb E e^{sM_n}\leq n\exp\!\left(\frac{\nu s^2}{2(1-cs)}\right).
$$

Applying [Jensen's inequality](../../../../jensen-s-inequality.md) to the [logarithm](../../../../logarithm.md) yields

$$
\mathbb EM_n\leq\frac1s\log\mathbb E e^{sM_n}
\leq\frac{\log n}{s}+\frac{\nu s}{2(1-cs)}.
$$

For $n>1$, put $a=\sqrt{2\log n/\nu}$ and choose $s=a/(1+ca)$. This gives $1-cs=1/(1+ca)$ and therefore

$$
\frac{\log n}{s}+\frac{\nu s}{2(1-cs)}
=\frac{\log n}{a}+c\log n+\frac{\nu a}{2}
=\sqrt{2\nu\log n}+c\log n.
$$

For $n=1$, let $s\downarrow0$ in the preceding upper bound, obtaining $\mathbb EX_1\leq0$. Consequently

$$
\boxed{\mathbb E\max_{1\leq i\leq n}X_i\leq\sqrt{2\nu\log n}+c\log n\quad(n\geq1).}
$$

The proof uses only the individual [moment-generating function](../../../../moment-generating-function.md) bounds for [Sub-Gamma random variables in the right tail](../../../../sub-gamma-random-variable-in-the-right-tail.md); it requires no [independence](../../../../independent-random-variables.md). Under the paper's literal one-sided definition, the negative part need not be integrable. The positive part of $M_n$ is integrable by the displayed exponential bound; if $\mathbb EM_n=-\infty$, the conclusion holds in the extended sense. Otherwise the application of [Jensen's inequality](../../../../jensen-s-inequality.md) is ordinary. Equivalently, truncate $M_n$ below and pass to the limit.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the algorithmic foundations of learning course of the University of Oxford](../../../split.md)
5. [Algorithmic foundations of learning course of the University of Oxford](../../../../algorithmic-foundations-of-learning-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
