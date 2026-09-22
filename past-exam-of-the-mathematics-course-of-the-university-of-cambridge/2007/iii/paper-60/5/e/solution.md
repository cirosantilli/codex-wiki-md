<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Take unilateral [Laplace transforms](../../../../../../laplace-transform.md) of the cavity equation, keeping the initial operator:

$$
(s+\gamma/2)\widetilde a(s)=a(0)-\sqrt\gamma\,\widetilde b_{\mathrm{in}}(s).
$$

The input-output relation gives

$$
\widetilde b_{\mathrm{out}}(s)=\widetilde b_{\mathrm{in}}(s)+\sqrt\gamma\,\widetilde a(s)
=\frac{s-\gamma/2}{s+\gamma/2}\widetilde b_{\mathrm{in}}(s)+\frac{\sqrt\gamma\,a(0)}{s+\gamma/2}.
$$

A [transfer function](../../../../../../transfer-function.md) describes the forced zero-state part of the response. Thus the [passive cavity input-output transfer function](../../../../../../passive-cavity-input-output-transfer-function.md) is

$$
\boxed{G(s)=\frac{s-\gamma/2}{s+\gamma/2}.}
$$

The omitted initial-state term is a decaying transient $\sqrt\gamma e^{-\gamma t/2}a(0)$, and is present for a general initial cavity state. This distinction avoids silently setting a physical annihilation operator equal to zero.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [5](../../5.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
