<h1 id="30d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set

$$
u=\log(1+t),
\qquad t=e^u-1,
\qquad dt=e^u\,du.
$$

Then

$$
J(x)=\int_0^{\log(1+\pi)}g(u)e^{-xu}\,du,
\qquad
g(u)=e^u\bigl[1-\cos(e^u-1)\bigr].
$$

The [Taylor series](../../../../../../taylor-series.md) at the endpoint is

$$
e^u-1=u+\frac{u^2}{2}+\frac{u^3}{6}+O(u^4),
$$

and hence

$$
g(u)=\frac{u^2}{2}+u^3+O(u^4).
$$

The [Watson lemma](../../../../../../watson-s-lemma.md), together with

$$
\int_0^\infty u^ne^{-xu}\,du=\frac{n!}{x^{n+1}},
$$

therefore yields

$$
\boxed{J(x)=\frac1{x^3}+\frac6{x^4}+O(x^{-5})}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30D](../../30d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
