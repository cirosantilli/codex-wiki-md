<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [Feynman rules](../../../../feynman-rules.md) and [Feynman gauge](../../../../feynman-gauge.md) convention from part [a](../a.md). Put $s=q^2$, $t=r_t^2$, $u=r_u^2$, the [Mandelstam variables](../../../../mandelstam-variables.md), and define the three-boson tensor with incoming [four-momenta](../../../../four-momentum.md) $(q,-k_1,-k_2)$:

$$
V^{\lambda\mu\nu}
=g^{\lambda\mu}(q+k_1)^\nu
+g^{\mu\nu}(k_2-k_1)^\lambda
-g^{\nu\lambda}(q+k_2)^\mu.
$$

The contributions, with external [Dirac spinors](../../../../dirac-spinor.md) included and both external [gauge boson](../../../../gauge-boson.md) [propagators](../../../../propagator.md) amputated, are

$$
\boxed{\begin{aligned}
\mathcal M_t^{ab\mu\nu}
&=-g^2\bar v(p_2)\,t^bt^a\gamma^\nu
\frac{\not r_t+m}{t-m^2+i0}\gamma^\mu u(p_1),\\
\mathcal M_u^{ab\mu\nu}
&=-g^2\bar v(p_2)\,t^at^b\gamma^\mu
\frac{\not r_u+m}{u-m^2+i0}\gamma^\nu u(p_1),\\
\mathcal M_s^{ab\mu\nu}
&=-ig^2\epsilon^{abc}\bar v(p_2)t^c\gamma_\lambda u(p_1)
\frac{V^{\lambda\mu\nu}}{s+i0},\\
\mathcal M^{ab\mu\nu}&=\mathcal M_t^{ab\mu\nu}
+\mathcal M_u^{ab\mu\nu}+\mathcal M_s^{ab\mu\nu}.
\end{aligned}}
$$

For example, $i\mathcal M_t$ contains $(+ig)^2i=-ig^2$. In the annihilation channel, the current vertex, [propagator](../../../../propagator.md), and three-boson vertex give $(+ig)(-i)g=g^2$, so division by the defining overall $i$ gives $-ig^2$. These relative signs are essential for the cancellation in part [d](../d.md). The antisymmetric colour factor makes the last expression symmetric under simultaneously exchanging $(a,\mu,k_1)$ and $(b,\nu,k_2)$, as required for identical outgoing [gauge bosons](../../../../gauge-boson.md). The [on shell](../../../../on-shell.md) external [Dirac spinors](../../../../dirac-spinor.md) obey $(\not p_1-m)u(p_1)=0$, $\bar v(p_2)(\not p_2+m)=0$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
