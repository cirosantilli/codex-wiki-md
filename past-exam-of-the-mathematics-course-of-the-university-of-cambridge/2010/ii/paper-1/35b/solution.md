<h1 id="35b/solution">Solution</h1>

↑ **Parent:** [35B](../35b.md)

The retarded [Green function](../../../../../green-s-function.md) for $\partial_t^2-\nabla^2$ in three dimensions is $G_{\rm ret}(x,t)=\delta(t-|x|)/(4\pi|x|)$. Radial reduction turns the homogeneous equation away from the origin into a one-dimensional outgoing wave for $rG$; the coefficient $1/(4\pi)$ is fixed by the small-sphere delta-source normalization. Convolution with $\mu_0j^\mu$ therefore solves the potential equation with vanishing incoming/initial field and gives

$$
A^\mu(x,t)=\frac{\mu_0}{4\pi}\int\frac{j^\mu(x',t-|x-x'|)}{|x-x'|}\,d^3x'.
$$

Current conservation ensures the [Lorenz gauge](../../../../../lorenz-gauge-condition.md): the divergence solves the homogeneous [wave equation](../../../../../wave-equation-split.md) with zero retarded data. Homogeneous radiation could be added if that physical boundary condition were not imposed.

Choose the edge $y=l/2$, directed along positive $x$. Put $d=\sqrt{z^2+l^2/4}$ and $t_*=\sqrt{z^2+l^2/2}$. Its retarded contribution on the axis is

$$
\mathbf A_{\rm edge}(z,t)=\frac{\mu_0I}{4\pi}\widehat x
\int_{-l/2}^{l/2}\frac{\Theta(t-\sqrt{s^2+d^2})}{\sqrt{s^2+d^2}}\,ds.
$$

The two symmetric halves are elementary inverse-hyperbolic integrals. Thus

$$
\boxed{\mathbf A_{\rm edge}=\frac{\mu_0I}{2\pi}\widehat x
\begin{cases}
0,&t<d,\\
\operatorname{arsinh}(\sqrt{t^2-d^2}/d),&d\leq t<t_*,\\
\operatorname{arsinh}(l/(2d)),&t\geq t_*.
\end{cases}}
$$

Reverse the direction for the opposite current orientation.

The closed loop's uniform switched current has zero spatial divergence, including at the corners, so it creates no charge accumulation. For the neutral loop and its current-induced field the retarded [scalar potential](../../../../../scalar-potential.md) is zero everywhere, not merely on the axis. At an axial point, opposite edges have identical retardation distances and opposite vector directions, so their vector potentials cancel at every time. Therefore

$$
\boxed{\mathbf E(0,0,z,t)=-\partial_t\mathbf A-\nabla\phi=0.}
$$

This cancellation holds distributionally at the wavefronts as well. Any independently prescribed initial electrostatic charge would contribute a separate field; it is not determined by the stated circulating current.

## ↑ Ancestors (10)

1. [35B](../35b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
