<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For $\alpha>0$, put $N(\alpha)=\lfloor\alpha^{-1}\rfloor$ and define the bounded operator

$$
R_\alpha
=\tau\sum_{n=0}^{N(\alpha)}
(I-\tau A^*A)^nA^*.
$$

Part (e) shows $R_\alpha f\to A^\dagger f$ for every $f\in\operatorname{dom}(A^\dagger)$ as $\alpha\downarrow0$. Since $\|I-\tau A^*A\|\leq1$,

$$
\|R_\alpha\|
\leq\tau(N(\alpha)+1)\|A\|.
$$

Choose the a priori rule

$$
\boxed{\alpha(\delta)=\sqrt\delta}.
$$

Then $N(\alpha(\delta))\to\infty$ while

$$
\delta\|R_{\alpha(\delta)}\|
\leq\tau\|A\|\delta(N(\alpha(\delta))+1)
\longrightarrow0.
$$

For $\|f^\delta-f\|\leq\delta$,

$$
\|R_{\alpha(\delta)}f^\delta-A^\dagger f\|
\leq
\delta\|R_{\alpha(\delta)}\|
+\|R_{\alpha(\delta)}f-A^\dagger f\|
\longrightarrow0.
$$

**Thus $\{R_\alpha\}$ with this parameter rule is a [regularization of an inverse problem](../../../../../../regularization-of-an-inverse-problem.md).**

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
