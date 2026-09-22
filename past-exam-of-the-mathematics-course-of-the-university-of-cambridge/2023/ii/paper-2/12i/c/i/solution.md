<h1 id="12i/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Since $\alpha$ generates $K^\times$, it cannot lie in a proper subfield, so its [minimal polynomial](../../../../../../../minimal-polynomial.md) over $\mathbb F_2$ has degree $d$. Write it as

$$
P(X)=X^d+c_{d-1}X^{d-1}+\cdots+c_1X+c_0.
$$

The identity $P(\alpha)=0$ and characteristic two give

$$
\alpha^d=\sum_{j=0}^{d-1}c_j\alpha^j.
$$

Multiplying by $\alpha^n$ and applying the linear map $T$ yields

$$
x_{n+d}=T(\alpha^{n+d})
=\sum_{j=0}^{d-1}c_jT(\alpha^{n+j})
=\sum_{j=0}^{d-1}c_jx_{n+j}.
$$

This is a binary linear recurrence of order at most $d$, so $(x_n)$ is the output of a [linear-feedback shift register](../../../../../../../linear-feedback-shift-register.md) of length at most $d$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [12I](../../../12i.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
