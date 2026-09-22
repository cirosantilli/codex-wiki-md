<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the [long-wave convection equation with broken Boussinesq symmetry](../../../../../../long-wave-convection-equation-with-broken-boussinesq-symmetry.md), use a sufficiently smooth real temperature field. To make the spatial average and integrations meaningful, take a periodic pattern, or an existing long-interval average with bounded derivatives and vanishing averaged endpoint fluxes. Boundedness of the temperature alone does not guarantee all those averaging properties. Multiply the evolution equation by $\Theta$ and average. [Integration by parts](../../../../../../integration-by-parts.md) gives

$$
\langle\Theta\Theta_{xx}\rangle=-\langle\Theta_x^2\rangle,\qquad
\langle\Theta\Theta_{xxxx}\rangle=\langle\Theta_{xx}^2\rangle,
$$

and $\langle\Theta(\Theta_x^j)_x\rangle=-\langle\Theta_x^{j+1}\rangle$. Thus the [energy method](../../../../../../energy-method.md) yields

$$
\boxed{\frac12\frac d{dt}\langle\Theta^2\rangle
=-\langle\Theta^2\rangle+\mu\langle\Theta_x^2\rangle
-\langle\Theta_{xx}^2\rangle+s\langle\Theta_x^3\rangle
-\langle\Theta_x^4\rangle.}
$$

The [energy square completion for long-wave convection](../../../../../../energy-square-completion-for-long-wave-convection.md) starts from

$$
\langle(\Theta+\Theta_{xx})^2\rangle
=\langle\Theta^2\rangle-2\langle\Theta_x^2\rangle
+\langle\Theta_{xx}^2\rangle\geq0.
$$

Put $v=\Theta_x$. The energy identity becomes

$$
\frac12\frac d{dt}\langle\Theta^2\rangle
=-\langle(\Theta+\Theta_{xx})^2\rangle
+\langle(\mu-2)v^2+sv^3-v^4\rangle.
$$

Since $sv-v^2=s^2/4-(v-s/2)^2\leq s^2/4$ pointwise,

$$
\boxed{\frac12\frac d{dt}\langle\Theta^2\rangle
\leq\langle(\mu-2)\Theta_x^2+s\Theta_x^3-\Theta_x^4\rangle
\leq(\mu-2+s^2/4)\langle\Theta_x^2\rangle.}
$$

Therefore **$\mu<2-s^2/4$ excludes growth of the mean-square temperature**, for arbitrary amplitude within this smooth averaging class. This is a nonlinear energy-stability criterion, not a proof of pointwise monotonicity at each position. A spatially constant component instead decays through the $-\Theta$ term. The criterion is sufficient; it need not coincide with the linear instability threshold.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
