<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The killed transition operator is

$$
P_tf(x)=\mathbb E_x[f(X_t)\mathbf1_{\{t<\mathcal T\}}]
=\int_0^1p(t,x,y)f(y)dy.
$$

The [infinitesimal generator](../../../../../../infinitesimal-generator-stochastic-processes.md) of the diffusion is

$$
L=\frac12\frac{d^2}{dx^2}+\frac12v(x)\frac d{dx}.
$$

The [Markov property](../../../../../../markov-property.md) and the [Chapman-Kolmogorov equation](../../../../../../chapman-kolmogorov-equation.md) give, for each fixed $y$,

$$
p(t+h,x,y)=\int_0^1p(h,x,z)p(t,z,y)dz
=P_h[p(t,\mathord\cdot,y)](x).
$$

Dividing by $h$, letting $h\downarrow0$, and using the generator definition together with the assumed $C^{1,2}$ regularity gives the pointwise [Kolmogorov backward equation](../../../../../../kolmogorov-backward-equation.md)

$$
\boxed{\partial_tp(t,x,y)
=\frac12\partial_x^2p(t,x,y)
+\frac12v(x)\partial_xp(t,x,y).}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
