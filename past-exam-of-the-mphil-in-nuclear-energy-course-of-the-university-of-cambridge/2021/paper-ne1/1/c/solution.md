<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Over $N$ [half-lives](../../../../../half-life.md), the duration is $T=Nt_{1/2}=N\ln2/\lambda$. The time-averaged thermal [power](../../../../../power.md) is

$$
\overline P=\frac1T\int_0^T P_0e^{-\lambda t}\,dt
=\frac{P_0}{\lambda T}(1-e^{-\lambda T}).
$$

Since $\lambda T=N\ln2$ and $e^{-\lambda T}=2^{-N}$,

$$
\boxed{\overline P=\frac{P_0}{N\ln2}(1-2^{-N}).}
$$

This is a time average, not the arithmetic mean of the initial and final powers. It follows directly from the assumed constant [nuclear decay constant](../../../../../nuclear-decay-constant.md) and constant recovered energy per decay.

## ↑ Ancestors (10)

1. [C](../c.md)
2. [1](../../1.md)
3. [Module NE1](../../../paper-ne1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../split.md)
6. [MPhil in nuclear energy course of the University of Cambridge](../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
