<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Let $Q(t)$ denote the [electric charge](../../../electric-charge-split.md) on the initially positive [capacitor](../../../capacitor.md) plate and define the discharge [electric current](../../../electric-current.md) by $I=-\dot Q$. [Kirchhoff's voltage law](../../../kirchhoff-cycle-law.md) for the [series RLC circuit](../../../series-rlc-circuit.md) gives the [damped harmonic oscillator](../../../damped-harmonic-oscillator.md) equation

$$
L\ddot Q+R\dot Q+\frac{Q}{C}=0.
$$

The initial conditions are $Q(0)=Q_0$ and $\dot Q(0)=0$: the open switch initially prevents [electric current](../../../electric-current.md), and finite [inductance](../../../inductance.md) prevents an instantaneous jump in it. Put $\gamma=R/(2L)$ and $\omega_0^2=1/(LC)$. The two [characteristic roots](../../../characteristic-root-of-a-constant-coefficient-differential-equation.md) are $s=-\gamma\pm\sqrt{\gamma^2-\omega_0^2}$. An oscillatory [electric current](../../../electric-current.md) requires a nonzero imaginary part, hence

$$
\boxed{R^2<\frac{4L}{C},\quad\text{or}\quad R<2\sqrt{\frac LC},\qquad \omega_d=\sqrt{\frac1{LC}-\frac{R^2}{4L^2}}.}
$$

For positive $L,C$ and nonnegative $R$, this is the [underdamped](../../../underdamping.md) regime. The initial conditions give

$$
Q(t)=Q_0e^{-\gamma t}\left(\cos\omega_dt+\frac{\gamma}{\omega_d}\sin\omega_dt\right),\qquad I(t)=\frac{Q_0}{LC\omega_d}e^{-\gamma t}\sin\omega_dt.
$$

At equality there is [critical damping](../../../critical-damping.md), and above it there is an [overdamped](../../../overdamping.md) response, with no repeated changes of sign of the discharge [electric current](../../../electric-current.md). A nonzero initial [electric charge](../../../electric-charge-split.md) is understood; if $Q_0=0$, the stated initial conditions give no [electric current](../../../electric-current.md) at all.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2015](../../2015-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
