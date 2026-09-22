<h1 id="12i/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Because $\alpha^{2^d-1}=1$,

$$
x_{n+2^d-1}=T(\alpha^{n+2^d-1})=T(\alpha^n)=x_n,
$$

so the period divides $2^d-1$.

Conversely, suppose $r$ is an eventual period. Then for every sufficiently large $n$,

$$
0=x_{n+r}-x_n
=T\bigl(\alpha^n(\alpha^r-1)\bigr).
$$

Any block of $2^d-1$ consecutive powers of $\alpha$ runs through every element of $K^\times$. Hence

$$
T\bigl((\alpha^r-1)y\bigr)=0
$$

for every $y\in K$, including $y=0$. The assumed [nondegenerate bilinear form](../../../../../../../nondegenerate-bilinear-form.md) forces $\alpha^r-1=0$. Since $\alpha$ generates the cyclic group $K^\times$ of order $2^d-1$, this means $2^d-1\mid r$. The least positive period is therefore

$$
\boxed{2^d-1},
$$

as in a [trace-generated maximal-period linear-feedback sequence](../../../../../../../trace-generated-maximal-period-linear-feedback-sequence.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
