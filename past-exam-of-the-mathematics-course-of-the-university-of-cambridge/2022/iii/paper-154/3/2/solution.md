<h1 id="3/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For real $h\in\mathcal D(\mathbb R^d)$, differentiation under the integral gives

$$
\left.\frac d{dt}E(Q+th)\right|_{t=0}
=\int\nabla Q\mathbin{\cdot}\nabla h-\int Q^{1+4/d}h.
$$

The ground-state equation $\Delta Q-Q+Q^{1+4/d}=0$ and [integration by parts](../../../../../../integration-by-parts.md) reduce this to

$$
\left.\frac d{dt}E(Q+th)\right|_{t=0}=-\int Qh.
$$

In particular, along the amplitude direction $h=Q$ the derivative is $-\|Q\|_2^2<0$. Hence $u_0=(1+\delta)Q$ has negative energy for every sufficiently small $\delta>0$, while

$$
\|u_0\|_2=(1+\delta)\|Q\|_2<\|Q\|_2+\epsilon
$$

when $\delta$ is chosen small enough. The ground state has finite variance, so [negative-energy blowup for the mass-critical focusing nonlinear Schrödinger equation](../../../../../../negative-energy-blowup-for-the-mass-critical-focusing-nonlinear-schrodinger-equation.md) shows that the corresponding solution blows up in finite time.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [3](../../3.md)
3. [Paper 154](../../../paper-154-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
