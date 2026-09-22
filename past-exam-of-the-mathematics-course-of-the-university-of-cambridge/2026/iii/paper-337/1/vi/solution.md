<h1 id="1/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

The energy-eigenstate expansion of $C(\tau)$ for $0<\tau<\beta$ is

$$
C(\tau)=\sum_{a,b}
p_a e^{-(E_b-E_a)\tau}|A_{ab}|^2.
$$

Fourier integration and $e^{i\omega_n\beta}=1$ give

$$
G(i\omega_n)
=\sum_{a,b}
\frac{p_a-p_b}{E_b-E_a-i\omega_n}|A_{ab}|^2.
$$

Comparing this with the spectral expression in part ii yields the [spectral representation of a thermal correlation function](../../../../../../spectral-representation-of-a-thermal-correlation-function.md)

$$
\boxed{
G(i\omega_n)
=-\int_{-\infty}^{\infty}
\frac{d\Omega}{\pi}\,
\frac{\operatorname{Im}G_R(\Omega)}
{\Omega-i\omega_n}}.
$$

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [1](../../1.md)
3. [Paper 337](../../../paper-337-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
