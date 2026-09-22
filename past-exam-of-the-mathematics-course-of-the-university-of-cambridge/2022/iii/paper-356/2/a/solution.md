<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Equation (1) is [Underdamped Langevin dynamics](../../../../../../underdamped-langevin-dynamics.md) for a unit-mass particle in potential $U$, coupled to a heat bath of temperature $T$. The coefficient $\gamma>0$ is viscous friction, and the noise amplitude is fixed by the [Fluctuation-dissipation theorem](../../../../../../fluctuation-dissipation-theorem.md). Its [Fokker-Planck equation](../../../../../../fokker-planck-equation.md) is

$$
\boxed{\partial_tf=-v\partial_xf
+\partial_v[(U'(x)+\gamma v)f]
+\gamma k_BT\partial_v^2f.}
$$

For $\gamma\gg1$, velocity relaxes rapidly, so formally

$$
V_tdt\simeq-\frac{U'(X_t)}\gamma dt
+\sqrt{\frac{2k_BT}{\gamma}}dW_t.
$$

Thus the [overdamped Langevin dynamics](../../../../../../overdamped-langevin-dynamics.md) is

$$
dX_t=-\phi'(X_t)dt+\sqrt{2D}\,dW_t,
\qquad D=\frac{k_BT}\gamma,
\qquad \phi=\frac U\gamma,
$$

and its density obeys

$$
\boxed{\partial_tp=\partial_x[D\partial_xp+\phi'(x)p].}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
