<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The original diagram has an ideal $5\,\mathrm V$ [electric battery](../../../electric-battery.md) feeding series [resistors](../../../resistor.md) of $8\,\Omega$ above the tapping point and $2\,\Omega$ below it. The long battery bar is positive, so terminal $A$ is above terminal $B$ in [electric potential](../../../electric-potential.md). With an [open circuit](../../../open-circuit.md) at the output, the internal [electric current](../../../electric-current.md) is $5/(8+2)=0.5\,\mathrm A$. The [voltage divider](../../../voltage-divider.md) therefore gives

$$
\boxed{\mathcal E_0=V_A-V_B=(0.5\,\mathrm A)(2\,\Omega)=1.0\,\mathrm V.}
$$

For the [Thévenin resistance](../../../thevenin-resistance.md), suppress the ideal voltage source by replacing it with a [short circuit](../../../short-circuit.md). The two [resistors](../../../resistor.md) are then in parallel as seen from $A,B$:

$$
\boxed{R_{\rm Th}=\frac{8\times2}{8+2}\,\Omega=1.6\,\Omega.}
$$

By [Thévenin's theorem](../../../thevenin-s-theorem.md), the terminal [voltage](../../../voltage.md) under an outward load [electric current](../../../electric-current.md) $I$ is $V_A-V_B=\mathcal E_0-IR_{\rm Th}$. Consequently

$$
\boxed{I_{\rm sc}=\frac{\mathcal E_0}{R_{\rm Th}}=0.625\,\mathrm A,}
$$

flowing through an external [short circuit](../../../short-circuit.md) from $A$ to $B$. Directly shorting the original terminals bypasses the $2\,\Omega$ [resistor](../../../resistor.md) and leaves $5\,\mathrm V$ across $8\,\Omega$, independently confirming the result.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2017 resit](../../2017-resit-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
