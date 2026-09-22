<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A convenient sufficient condition is that $f\in C^2(\mathbb R^d)$ has a bounded [gradient](../../../../../gradient.md). The [Itô formula](../../../../../ito-s-lemma.md) for standard $d$-dimensional [Brownian motion](../../../../../brownian-motion-split.md) gives

$$
f(B_t)-\frac12\int_0^t\Delta f(B_s)\,ds
=f(0)+\sum_{j=1}^d\int_0^t\partial_jf(B_s)\,dB_s^j.
$$

If $|\nabla f|\leq C$, the [Itô isometry](../../../../../ito-isometry.md) gives

$$
\mathbb E\left|\sum_j\int_0^t\partial_jf(B_s)\,dB_s^j\right|^2
=\mathbb E\int_0^t|\nabla f(B_s)|^2\,ds\leq C^2t.
$$

Thus the right side is a [square-integrable](../../../../../square-integrable-function.md) [martingale](../../../../../martingale-split.md), rather than merely a [local martingale](../../../../../local-martingale.md). In particular,

$$
\boxed{f\in C^2(\mathbb R^d),\quad \sup_x|\nabla f(x)|<\infty
\quad\Longrightarrow\quad M^f\text{ is a martingale}.}
$$

There are many nonconstant examples, such as $f(x)=\sin x_1$ or $f(x)=x_1$. More generally it is enough that $\mathbb E\int_0^t|\nabla f(B_s)|^2ds<\infty$ for each finite $t$. Smooth [test functions](../../../../../test-function.md) with [compact support](../../../../../compact-support.md) satisfy the bounded-gradient condition and will provide the domain in the next part.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the stochastic differential equations course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations course of the University of Oxford](../../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
