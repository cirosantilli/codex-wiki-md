<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Remove the [quadratic phase](../../../../../../quadratic-phase.md) by setting

$$
g(x)=f(x)\omega^{-x^2}.
$$

The phase around the parallelogram is

$$
-x^2+(x-a)^2+(x-b)^2-(x-a-b)^2=-2ab,
$$

so the hypothesis says exactly that $\|g\|_{U^2}^4\geq c$, with harmless negative choices of the increments. The Fourier identity for the [Gowers U2 norm](../../../../../../gowers-u2-norm.md) and the [Parseval identity](../../../../../../parseval-identity.md) now give

$$
c\leq\sum_r|\widehat g(r)|^4
\leq\left(\max_r|\widehat g(r)|^2\right)\sum_r|\widehat g(r)|^2
=\left(\max_r|\widehat g(r)|^2\right)\mathbb E_x|g(x)|^2
\leq\max_r|\widehat g(r)|^2,
$$

where the last inequality uses $\|f\|_\infty\leq1$. Thus the [Quadratic phase detection by the Gowers U2 norm](../../../../../../quadratic-phase-detection-by-the-gowers-u2-norm.md) supplies an $r\in\mathbb Z_N$ such that

$$
\boxed{\left|\mathbb E_xf(x)\omega^{-rx-x^2}\right|=|\widehat g(r)|\geq c^{1/2}.}
$$

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 147](../../../paper-147-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
