<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $f_\epsilon(x)=(\epsilon^2+x^2)^{1/2}$, direct [differentiation](../../../../../../differentiation.md) gives

$$
f_\epsilon'(x)=\frac{x}{\sqrt{\epsilon^2+x^2}},
\qquad
f_\epsilon''(x)=\frac{\epsilon^2}{(\epsilon^2+x^2)^{3/2}}.
$$

Since the [quadratic variation](../../../../../../quadratic-variation.md) of standard [Brownian motion](../../../../../../brownian-motion-split.md) is $[B]_t=t$, the [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
\boxed{f_\epsilon(B_t)=\epsilon+
\int_0^t\frac{B_s}{\sqrt{\epsilon^2+B_s^2}}\,dB_s
+\frac12\int_0^t\frac{\epsilon^2}{(\epsilon^2+B_s^2)^{3/2}}\,ds.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
