<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The condition $\sum_{i=1}^n1/p_i=1$ and positivity imply $p_i\geq1$. We prove the [Generalized Holder inequality](../../../../../../generalized-holder-inequality.md) by induction on $n$. The case $n=2$ is the usual [Holder inequality](../../../../../../holder-inequality.md). For the induction step, set

$$
\frac1q=\sum_{i=1}^{n-1}\frac1{p_i}=1-\frac1{p_n}.
$$

The exponents $q$ and $p_n$ are conjugate, so Hölder followed by the induction hypothesis gives

$$
\begin{aligned}
\left\|\prod_{i=1}^nf_i\right\|_1
&\leq\left\|\prod_{i=1}^{n-1}f_i\right\|_q\|f_n\|_{p_n}\\
&\leq\prod_{i=1}^n\|f_i\|_{p_i}.
\end{aligned}
$$

This proves the claim.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
