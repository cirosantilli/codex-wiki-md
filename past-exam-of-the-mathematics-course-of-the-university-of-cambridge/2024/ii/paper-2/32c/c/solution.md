<h1 id="32c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Repeated integration by parts starts with

$$
\operatorname{si}(x)
=\frac{\cos x}{x}
-\frac1x\int_1^\infty\frac{\cos(xt)}{t^2}\,dt
=\frac{\cos x}{x}+\frac{\sin x}{x^2}
-\frac2{x^2}\int_1^\infty\frac{\sin(xt)}{t^3}\,dt.
$$

Continuing alternates sine and cosine and multiplies by successive integers. After finitely many steps the remainder is bounded by a constant times the next inverse power, so the [fixed-lower-limit sine-integral expansion](../../../../../../fixed-lower-limit-sine-integral-expansion.md) is

$$
\operatorname{si}(x)\sim
\cos x\sum_{n=0}^\infty(-1)^n(2n)!x^{-2n-1}
+\sin x\sum_{n=0}^\infty(-1)^n(2n+1)!x^{-2n-2}.
$$

Therefore

$$
\boxed{a_n=(-1)^n(2n)!,\qquad
b_n=(-1)^n(2n+1)!}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [32C](../../32c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
