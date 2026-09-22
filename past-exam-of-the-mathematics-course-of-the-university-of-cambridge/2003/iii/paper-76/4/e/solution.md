<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Because $\zeta<\eta\leq h(x)$, the lower layer is saturated along the entire barrier. Both layers have the same horizontal head gradient but different [Darcy velocities](../../../../../../darcy-velocity.md). Integrating their conductivity over the actual cross-section gives the transmissivity

$$
\mathcal T(h)=\frac{\rho g}{\mu}\left[k_1\frac{\alpha\zeta^3}{3}
+k_2\frac{\alpha(h^3-\zeta^3)}{3}\right]
=\frac{\rho g\alpha}{3\mu}\left[k_2h^3+(k_1-k_2)\zeta^3\right].
$$

The total discharge is $Q=-\mathcal T(h)h_x$. Hence $QL=\int_\eta^H\mathcal T(h)dh$, giving

$$
\boxed{Q=\frac{\rho g\alpha}{3\mu L}
\left[\frac{k_2}{4}(H^4-\eta^4)+(k_1-k_2)\zeta^3(H-\eta)\right].}
$$

This is a parallel-layer conductivity integral, not a series-resistance average: the layers share the horizontal pressure drop. It reduces to the previous result when $k_1=k_2$. The assumption $\zeta<\eta$ is important; if the downstream free surface cuts the lower layer, the transmissivity and its head integration must be split into different saturation regimes.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
