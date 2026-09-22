<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Analytically continue the free-particle return kernel using $M=I$ and $t=-i\hbar\beta$. This fixes

$$
\boxed{\mathcal Z_0=\sqrt{\frac{I}{2\pi\hbar^2\beta}}.}
$$

Set $a=2\pi^2I/(\hbar^2\beta)$. The Gaussian Fourier integral in [Poisson resummation](../../../../../../poisson-summation-formula.md) is

$$
\int_{-\infty}^\infty dx\,e^{-ax^2+2\pi inx}=\sqrt{\frac\pi a}\,e^{-\pi^2n^2/a}.
$$

Applying it to the winding sum gives $\sum_me^{-am^2}=\sqrt{\pi/a}\sum_ne^{-\pi^2n^2/a}$. The prefactors cancel exactly, $2\pi\mathcal Z_0\sqrt{\pi/a}=1$, and $\pi^2/a=\beta\hbar^2/(2I)$. Therefore

$$
\boxed{\mathcal Z=\sum_{n\in\mathbb Z}e^{-\beta\hbar^2n^2/(2I)},}
$$

in agreement with the spectral trace. This is [momentum-winding duality of the quantum rotor](../../../../../../momentum-winding-duality-of-the-quantum-rotor.md). At low temperature the momentum [ground state](../../../../../../ground-state.md) dominates; at high temperature the winding-zero sector gives $\mathcal Z\simeq\sqrt{2\pi I/(\beta\hbar^2)}$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
