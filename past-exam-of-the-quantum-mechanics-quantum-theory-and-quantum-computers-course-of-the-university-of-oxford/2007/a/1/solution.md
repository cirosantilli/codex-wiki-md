<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Differentiate the [Lagrangian](../../../../lagrangian.md) with respect to the generalized velocities:

$$
\boxed{p_j=\frac{\partial L}{\partial\dot x_j}=m\dot x_j+eA_j.}
$$

The [Legendre transform](../../../../convex-conjugate.md) cancels the vector-[potential energy](../../../../potential-energy.md) term, giving $H=p\cdot\dot x-L=m|\dot x|^2/2+V$. Eliminating [velocity](../../../../velocity.md) with $m\dot x=p-eA$ therefore yields

$$
\boxed{H=\frac{|p-eA|^2}{2m}+V.}
$$

For the given gauge, set $\pi_1=p_1+eBx_2/2$, $\pi_2=p_2-eBx_1/2$, $\pi_3=p_3$. [Hamilton's equations](../../../../hamilton-s-equations.md) give $\dot x_j=\pi_j/m$, $\dot p_1=(eB/2)\dot x_2$, $\dot p_2=-(eB/2)\dot x_1$, $\dot p_3=0$. Hence the conserved quantities are

$$
\boxed{p_3,\qquad K_1=p_1-\frac{eB}{2}x_2,\qquad K_2=p_2+\frac{eB}{2}x_1,\qquad H.}
$$

The two transverse combinations are components of [magnetic pseudomomentum](../../../../magnetic-pseudomomentum.md). **The printed conserved combinations omit the [electric charge](../../../../electric-charge-split.md) factor $e$.** With the stated [vector potential](../../../../vector-potential.md) and general [electric charge](../../../../electric-charge-split.md) they need the factors displayed above; as printed they hold only if $e=1$ or if [electric charge](../../../../electric-charge-split.md) is already absorbed into the field convention.

The initial data give $K_1=K_2=p_3=0$. Thus $p_1=eBx_2/2$, $p_2=-eBx_1/2$ throughout, and

$$
\dot x_1=\omega_cx_2,\qquad\dot x_2=-\omega_cx_1,\qquad\omega_c=eB/m.
$$

Solving with the initial point gives

$$
\boxed{x_1=a\sin(\omega_ct),\quad x_2=a\cos(\omega_ct),\quad x_3=0.}
$$

Consequently $x_1^2+x_2^2=a^2$: the [guiding centre](../../../../guiding-center.md) is the origin and the signed [cyclotron frequency](../../../../cyclotron-frequency.md) fixes the rotation direction. The [energy](../../../../energy-split.md) is the constant $e^2B^2a^2/(2m)$.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../split.md)
5. [Quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../../quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
