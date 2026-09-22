<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $f$ be [probability density](../../../../../probability-density.md) per unit solid angle, with $\int_{S^2}f\,d\Omega=1$ and isotropic initial condition $f(\mathbf p,0)=1/(4\pi)$. In still fluid, [bottom-heavy spherical-cell orientation dynamics](../../../../../bottom-heavy-spherical-cell-orientation-dynamics.md) gives $\dot{\mathbf p}=B^{-1}[\mathbf k-(\mathbf k\cdot\mathbf p)\mathbf p]$. Adding isotropic rotational [diffusion](../../../../../diffusion.md) gives the [gyrotactic orientation Fokker-Planck equation](../../../../../gyrotactic-orientation-fokker-planck-equation.md)

$$
\partial_tf+\nabla_p\cdot(f\dot{\mathbf p})=D_r\Delta_{S^2}f.
$$

The derivatives are tangential to the unit sphere. Rotational symmetry about $\mathbf k$ is preserved by both the equation and the initial condition, so $f$ depends only on $\theta,t$. Since $\dot\theta=-\sin\theta/B$, the polar probability flux is $j_\theta=-\sin\theta f/B-D_rf_\theta$. Expanding $\partial_tf+\sin^{-1}\theta\,\partial_\theta(\sin\theta j_\theta)=0$ yields

$$
\boxed{Bf_t-\sin\theta f_\theta-2\cos\theta f
=\frac{BD_r}{\sin\theta}\partial_\theta(\sin\theta f_\theta).}
$$

Regular solutions have no probability flux through the poles. The mean swimming [velocity](../../../../../velocity.md) is $\mathbf V_c=V_s\langle\mathbf p\rangle$, with only a vertical component by symmetry.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 81](../../paper-81-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
