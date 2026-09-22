<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Since $n_0=qn_k$ and the $k$ experimental arms each contain $n_k$ patients,

$$
n_k=\frac{n_{\mathrm{tot}}}{k+q}.
$$

Consequently

$$
V=\frac1{n_0}+\frac1{n_k}
=\frac{(q+1)(q+k)}{qn_{\mathrm{tot}}}
=\frac{q+k+1+k/q}{n_{\mathrm{tot}}}.
$$

Differentiation gives $V'(q)=(1-k/q^2)/n_{\mathrm{tot}}$, so the stationary point is $q=\sqrt k$. Since

$$
V''(q)=\frac{2k}{q^3n_{\mathrm{tot}}}>0,
$$

this is the unique minimum. Thus a shared standard arm should be $\sqrt k$ times the size of each new-treatment arm.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
