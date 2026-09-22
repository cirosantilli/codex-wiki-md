<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $\tau=\tau_1+i\tau_2$ and $q=e^{2\pi i\tau}$. The torus partition function is the [trace](../../../../../../matrix-trace.md)

$$
Z(\tau,\bar\tau)=\operatorname{Tr}
e^{-2\pi\tau_2H+2\pi i\tau_1P}.
$$

The continuum momentum states have density $V/(2\pi)$, so their contribution is

$$
\frac V{2\pi}\int_{-\infty}^{\infty}dp\,e^{-\pi\tau_2p^2}
=\frac V{2\pi\sqrt{\tau_2}}.
$$

Each left-moving oscillator contributes $\sum_{N\geq0}q^{nN}=(1-q^n)^{-1}$, with the complex conjugate for the right mover. The zero-point factor combines these products into the [Dedekind eta function](../../../../../../dedekind-eta-function.md)

$$
\eta(\tau)=q^{1/24}\prod_{n=1}^{\infty}(1-q^n).
$$

Therefore the [torus partition function of a free boson](../../../../../../torus-partition-function-of-a-free-boson.md) is

$$
\boxed{Z(\tau,\bar\tau)=\frac V{2\pi\sqrt{\operatorname{Im}\tau}}
|\eta(\tau)|^{-2}}.
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 306](../../../paper-306-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
