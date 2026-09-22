<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Here $h(x)$ attains its maximum one at $x=1$, so $a=1$. For $x\leq0$, put $t=-x\geq0$. Then $x^2h(x)=e^{-1/2}t^2e^{-t/2}$. Its derivative is $e^{-1/2}e^{-t/2}t(2-t/2)$, so its maximum is at $t=4$, with value $16e^{-5/2}$.

For $0\leq x\leq1$, $x^2h(x)=x^2e^{(x-1)/2}$ is increasing and has maximum one. For $x\geq1$, $x^2h(x)=x^2e^{-(x-1)/2}$ has logarithmic derivative $2/x-1/2$, so its maximum is at $x=4$, with value $16e^{-3/2}>1$. Therefore the [Laplace ratio-of-uniforms envelope](../../../../../../../laplace-ratio-of-uniforms-envelope.md) has the finite bounds

$$
\boxed{a=1,\qquad b_1=-4e^{-5/4},\qquad b_2=4e^{-3/4}.}
$$

These calculations establish finiteness and identify the tight axis-aligned bounds, rather than relying only on exponential tail decay.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
