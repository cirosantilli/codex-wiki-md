<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Fix the standard [Jacobian matrix](../../../../../../jacobian-matrix.md) convention $(Da)_{ij}=\partial_{v_j}a_i$. With column [gradients](../../../../../../gradient.md), the [commuting velocity derivative for kinetic transport](../../../../../../commuting-velocity-derivative-for-kinetic-transport.md) is

$$
\boxed{G=\nabla_v f+t(Da)^T\nabla_x f.}
$$

If the symbol $J_a$ is instead defined with derivative indices as rows, the printed expression is this same formula. Under the standard convention it needs a transpose.

To prove the claim, put $D=\partial_t+a(v)\cdot\nabla_x$. Differentiating $Df=0$ in $v_j$ gives

$$
D(\partial_{v_j}f)=-\sum_i(\partial_{v_j}a_i)\partial_{x_i}f,
\qquad
D\left(t\sum_i(\partial_{v_j}a_i)\partial_{x_i}f\right)
=\sum_i(\partial_{v_j}a_i)\partial_{x_i}f.
$$

The terms cancel, so each component of $G$ satisfies the [transport equation](../../../../../../transport-equation.md). Multiplication by the smooth coefficient $Da$ and differentiation preserve the same uniform [compact support](../../../../../../compact-support.md), hence $G\in\mathcal C_T$ componentwise. At $t=0$, $G(0)=\nabla_v f_{\mathrm{in}}$. The [L2 norm](../../../../../../l2-norm.md) calculation in part (d), summed over components, gives

$$
\boxed{\int|T(Da)^T\nabla_xf(T)+\nabla_vf(T)|^2\,dx\,dv
=\int|\nabla_vf_{\mathrm{in}}|^2\,dx\,dv.}
$$

One can also differentiate the explicit solution: the $t(Da)^T\nabla_x f$ term cancels the derivative of $x-ta(v)$, leaving the initial velocity derivative transported along the [characteristic curves](../../../../../../characteristic-curve.md).

The transpose matters. For the shear $a(v)=(v_1+v_2,v_2)$, $\det Da=1$ but $Da\ne(Da)^T$. The printed field satisfies $Dg=(Da-(Da)^T)\nabla_xf$, which is nonzero for a generic compactly supported datum. **The untransposed formula is false with the standard convention.**

## ↑ Ancestors (11)

1. [G](../g.md)
2. [1](../../1.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
