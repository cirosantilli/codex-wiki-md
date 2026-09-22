<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Label the [capacitor](../../../../capacitor.md)'s left terminal $a$ and right terminal $b$, with the battery's negative node at zero. The source diagram has $2R$ from $a$ to ground, $R$ from $b$ to ground, and a source-side [resistor](../../../../resistor.md) $R$ feeding $a$ from [electric potential difference](../../../../electric-potential-difference.md) $V$. The [capacitor](../../../../capacitor.md) [electric current](../../../../electric-current.md) $I_2$ flows from $a$ to $b$; $I_1$ flows through $2R$.

With the [capacitor](../../../../capacitor.md) removed, $V_a=2V/3$ and $V_b=0$, so the [Thévenin equivalent](../../../../thevenin-equivalent.md) seen by the [capacitor](../../../../capacitor.md) has $V_{\rm th}=2V/3$. Suppress the ideal [electric potential difference](../../../../electric-potential-difference.md) source to find its [electrical resistance](../../../../electrical-resistance.md): the left terminal sees $R\parallel2R=2R/3$ to ground and the right sees $R$, giving $R_{\rm th}=5R/3$ between the terminals.

The initially uncharged [capacitor](../../../../capacitor.md) [electric potential difference](../../../../electric-potential-difference.md) $V_C=V_a-V_b$ therefore obeys

$$
R_{\rm th}C\frac{dV_C}{dt}+V_C=V_{\rm th},\qquad V_C(0)=0.
$$

Solving gives $V_C=(2V/3)(1-e^{-t/\tau})$, with $\tau=R_{\rm th}C$. The [capacitor](../../../../capacitor.md) [electric current](../../../../electric-current.md) is $I_2=C\dot V_C$, hence

$$
\boxed{I_2(t)=\frac{2V}{5R}e^{-t/\tau},\qquad A=\frac{2V}{5R},\qquad\tau=\frac{5RC}{3}}.
$$

At $t=0^+$, the short-like uncharged [capacitor](../../../../capacitor.md) makes $V_a=V_b=2V/5$, so $I_2=2V/(5R)$ directly from the right [resistor](../../../../resistor.md). At long times the [capacitor](../../../../capacitor.md) carries no direct [electric current](../../../../electric-current.md). These endpoint checks agree with the exponential solution.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [9](../../9.md)
3. [2015 resit](../../../2015-resit-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
