<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply [Itô formula](../../../../../../ito-s-lemma.md) to $\phi(x)=x\log x$. Since $\phi''(x)=1/x$,

$$
M_1\log M_1-M_0\log M_0
=\int_0^1(1+\log M_t)\,dM_t
+\frac12\int_0^1\frac{d[M]_t}{M_t}.
$$

Boundedness of $\log M$ makes the stochastic integral a true martingale of mean zero. Taking expectations proves

$$
\boxed{\mathbb E(M_1\log M_1)=\mathbb E(M_0\log M_0)+\frac12\mathbb E\int_0^1\frac{d[M]_t}{M_t}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
