<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The time-domain [Feynman rules](../../../../../../feynman-rule.md) are:

- each internal line joining times $t,t'$ contributes $D(t-t')$;
- each cubic vertex contributes $-i\lambda$ and an integration $\int dt$;
- divide by the graph's [Feynman-diagram symmetry factor](../../../../../../feynman-diagram-symmetry-factor.md);
- attach the external times to the corresponding lines and retain connected graphs.

There is no order-$\lambda$ connected two-point correction. Through order $\lambda^2$, the two connected topologies are the two-vertex fish graph and the one-particle-reducible tadpole graph. With the displayed vertex convention,

$$
\begin{aligned}
\langle T x(t_1)x(t_2)\rangle_{\mathrm{conn}}
={}&D(t_1-t_2)\\
&+\frac{(-i\lambda)^2}{2}\int dt\,dt'\,
D(t_1-t)D(t-t')^2D(t'-t_2)\\
&+\frac{(-i\lambda)^2}{2}\int dt\,dt'\,
D(t_1-t)D(t_2-t)D(t-t')D(0)
+O(\lambda^4),
\end{aligned}
$$

up to the common factors of $i$ associated with the propagator convention. Vacuum normalization removes disconnected vacuum bubbles.

These integrals are ultraviolet finite in one time dimension: a harmonic-oscillator propagator behaves as $E^{-2}$ at large frequency, and the loop-frequency integrals have negative superficial degree of divergence. They are also infrared finite because $\omega>0$ supplies a gap. The cubic instability affects nonperturbative convergence but does not create a divergence in these fixed-order integrals.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
