<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\delta=\sqrt{2\eta/\omega}$ and $q=(1+i)/\delta$. Within the [magnetic skin layer](../../../../../../magnetic-skin-layer.md), differentiation across the layer dominates differentiation along the wall by the factor $b/\delta$. The leading [resistive induction equation](../../../../../../resistive-induction-equation.md) is therefore

$$
i\omega B_x=\eta\partial_y^2B_x,\qquad B_x(x,0)=C(x),\qquad B_x\longrightarrow0\quad(y/\delta\longrightarrow\infty).
$$

Because $\eta q^2=i\omega$ and $\operatorname{Re}q>0$, its decaying solution is

$$
\boxed{B_x=C(x)e^{-qy},\qquad B_z=0.}
$$

The [solenoidal magnetic-field constraint](../../../../../../solenoidal-magnetic-field-constraint.md) determines the first smaller component,

$$
B_y=\frac{C'(x)}q e^{-qy},\qquad \frac{B_y}{B_x}=O(\delta/b).
$$

Corrections to $B_x$ from longitudinal diffusion have relative order $(\delta/b)^2$. Thus the zero normal boundary field from the [perfect conductor](../../../../../../perfect-conductor.md) calculation is a leading-order condition, not an additional exact condition at finite $\eta$. A smaller exterior-field correction matches $B_y$.

To leading order the [electric current density](../../../../../../current-density.md) is $j_z=qCe^{-qy}/\mu_0$. For two real harmonic fields, the period average of their product is half the real part of the product of one amplitude with the conjugate of the other. Thus the [mean Lorentz force in a magnetic skin layer](../../../../../../mean-lorentz-force-in-a-magnetic-skin-layer.md) is

$$
\overline{\mathbf F}=\frac1{2\mu_0}\operatorname{Re}\{(\nabla\times\mathbf B)\times\mathbf B^*\}.
$$

Its normal component is

$$
\boxed{\overline F_y=\frac{C(x)^2}{2\mu_0\delta}e^{-2y/\delta},\qquad \overline{\mathbf F}=\overline F_y\mathbf e_y\quad\hbox{to leading order}.}
$$

The first possible tangential contribution from the smaller $B_y$ vanishes: it is $-CC'e^{-2y/\delta}\operatorname{Re}(q/q^*)/(2\mu_0)$, and $q/q^*=i$. This cancellation matters in computing the tangential streaming flow.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
