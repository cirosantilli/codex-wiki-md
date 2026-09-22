<h1 id="15b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Conformal time](../../../../../../conformal-time.md) is defined by

$$
d\tau=\frac{dt}{a(t)}.
$$

For $a=a_0e^{H_{\rm inf}t}$, choose $\tau\to0$ as $t\to+\infty$. Integration gives

$$
\boxed{
\tau=-\frac{e^{-H_{\rm inf}t}}{a_0H_{\rm inf}}
=-\frac1{aH_{\rm inf}},
\qquad -\infty<\tau<0
},
$$

as recorded by [Conformal time during de Sitter expansion](../../../../../../conformal-time-during-de-sitter-expansion.md).

Writing a prime for $d/d\tau$, the relations

$$
\frac d{dt}=\frac1a\frac d{d\tau},
\qquad
\frac{a'}a=-\frac1\tau
$$

turn the Fourier-mode equation into

$$
\widehat\phi_{\mathbf k}''
+2\frac{a'}a\widehat\phi_{\mathbf k}'
+c^2k^2\widehat\phi_{\mathbf k}=0.
$$

Set

$$
\widetilde\phi_{\mathbf k}
=a\widehat\phi_{\mathbf k}
=-\frac1{H_{\rm inf}\tau}\widehat\phi_{\mathbf k}.
$$

A direct substitution gives

$$
\widetilde\phi_{\mathbf k}''
+\left(c^2k^2-\frac{a''}a\right)
\widetilde\phi_{\mathbf k}=0.
$$

Here $a''/a=2/\tau^2$, so the [Canonically rescaled de Sitter scalar mode](../../../../../../canonically-rescaled-de-sitter-scalar-mode.md) obeys

$$
\boxed{
\frac{d^2\widetilde\phi_{\mathbf k}}{d\tau^2}
+\left(c^2k^2-\frac2{\tau^2}\right)
\widetilde\phi_{\mathbf k}=0
}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [15B](../../15b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
