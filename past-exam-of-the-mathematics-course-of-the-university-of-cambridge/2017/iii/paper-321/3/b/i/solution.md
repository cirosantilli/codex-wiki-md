<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [pressureless dust fluid in a shearing sheet](../../../../../../../pressureless-dust-fluid-in-a-shearing-sheet.md) has no [pressure](../../../../../../../pressure.md) restoration and is driven by [drag force](../../../../../../../drag-physics.md) toward the prescribed gas velocity; gas backreaction is omitted in the given model. After linearizing about the common background shear, axisymmetry gives

$$
(\partial_t+\epsilon\Omega)v'_x-2\Omega v'_y=\epsilon\Omega u'_x,\qquad (\partial_t+\epsilon\Omega)v'_y+\frac\Omega2v'_x=\epsilon\Omega u'_y.
$$

Apply $D_\epsilon=\partial_t+\epsilon\Omega$ to the first equation and use the second to eliminate $v'_y$. The exact linear scalar equation is

$$
\bigl[\partial_t^2+2\epsilon\Omega\partial_t+(1+\epsilon^2)\Omega^2\bigr]v'_x=\epsilon\Omega\partial_tu'_x+\epsilon^2\Omega^2u'_x+2\epsilon\Omega^2u'_y.
$$

For the supplied leading-order epicycle, set $\theta=kx-\Omega t$. Since $\partial_tu'_x=\Omega u\sin\theta$ and $u'_y=u\sin\theta/2$, this becomes

$$
\boxed{\partial_t^2v'_x+2\epsilon\Omega\partial_tv'_x+(1+\epsilon^2)\Omega^2v'_x=2\epsilon\Omega^2u\sin\theta+\epsilon^2\Omega^2u\cos\theta.}
$$

The final cosine term is missing from the printed equation. Dropping it is justified at leading order in $0<\epsilon\ll1$, recovering the intended forcing, but the printed equation retains an order-$\epsilon^2$ frequency term on the left and is not an exact derivation at that order. A direct countercheck is $\mathbf v'=\mathbf u'$: the drag vanishes and the pair solves both dust equations exactly, while $v'_x=u\cos\theta$ leaves residual $\epsilon^2\Omega^2u\cos\theta$ in the printed scalar equation. This is the [forced dust epicycle with aerodynamic drag](../../../../../../../forced-dust-epicycle-with-aerodynamic-drag.md); its damping time is $(\epsilon\Omega)^{-1}$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 321](../../../../paper-321-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
