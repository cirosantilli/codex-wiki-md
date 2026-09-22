<h1 id="31j/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A function in the stated network class has the form

$$
f(x)=\sum_{j=1}^m\alpha_j\operatorname{sgn}(x^T\beta_j).
$$

Thus this is the class $\mathcal F_2$ from part (d), with the hidden-unit class

$$
\mathcal G=\mathcal H_{\mathcal F_1}.
$$

Parts (c) and (d) give

$$
\begin{aligned}
s(\mathcal H_{\mathcal F_3},n)
&\leq(n+1)^m s(\mathcal G,n)^m\\
&\leq(n+1)^m\bigl((n+1)^p\bigr)^m\\
&=\boxed{(n+1)^{(p+1)m}}.
\end{aligned}
$$

This is the [growth bound for a single-hidden-layer sign network](../../../../../../growth-bound-for-a-single-hidden-layer-sign-network.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [31J](../../31j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
