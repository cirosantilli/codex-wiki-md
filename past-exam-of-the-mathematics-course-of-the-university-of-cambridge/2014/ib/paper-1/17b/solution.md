<h1 id="17b/solution">Solution</h1>

↑ **Parent:** [17B](../17b.md)

The steady [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md) with no body force are $(\mathbf u\cdot\nabla)\mathbf u=-\nabla p/\rho$. Use the [convective acceleration identity](../../../../../convective-acceleration-identity.md)

$$
(\mathbf u\cdot\nabla)\mathbf u=\nabla(\tfrac12|\mathbf u|^2)-\mathbf u\times(\nabla\times\mathbf u)
$$

to obtain

$$
\boxed{\mathbf u\times\boldsymbol\omega=\nabla\left(\frac p\rho+\tfrac12|\mathbf u|^2\right).}
$$

For the question's [streamfunction](../../../../../stream-function.md) convention, $\mathbf u=(\psi_y,-\psi_x,0)$, so $\mathbf u\times\boldsymbol\omega=-\omega\nabla\psi$. Constant $\omega$ therefore gives the [Bernoulli function for planar constant-vorticity flow](../../../../../bernoulli-function-for-planar-constant-vorticity-flow.md)

$$
\boxed{\tfrac12|\mathbf u|^2+\omega\psi+p/\rho=C}
$$

on the connected fluid region.

For circular [streamlines](../../../../../streamline.md), write $\mathbf u=w(r)\widehat{\boldsymbol\phi}$. The cylindrical [curl](../../../../../curl.md) gives $(rw)'/r=\omega$, so $w=\omega r/2+C_1/r$. The outer wall condition gives $C_1=-2\omega a^2$. Choose the positive azimuthal orientation so that $w(a)=V$, as implicit in the requested sign for $\omega$. Then

$$
\boxed{\omega=-\frac{2V}{3a},\qquad \mathbf u=\frac V{3a}\left(\frac{4a^2}{r}-r\right)\widehat{\boldsymbol\phi}.}
$$

Reversing the circulation reverses $\omega$ but leaves the speed and pressure difference unchanged. For this [uniform-vorticity circular flow in an annulus](../../../../../uniform-vorticity-circular-flow-in-an-annulus.md), one convenient streamfunction is $\psi=V(r^2/2-4a^2\log(r/a))/(3a)+C_2$.

The radial component of the [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md) is $p_r=\rho w^2/r$. Thus pressure increases outwards, and

$$
\begin{aligned}
p(2a)-p(a)&=\frac{\rho V^2}{9a^2}\int_a^{2a}\left(\frac{16a^4}{r^3}-\frac{8a^2}{r}+r\right)\,dr\\
&=\frac{\rho V^2}{9a^2}\left[\frac{15a^2}{2}-8a^2\log2\right].
\end{aligned}
$$

Therefore

$$
\boxed{\Delta p=p(2a)-p(a)=\frac{15-16\log2}{18}\rho V^2.}
$$

## ↑ Ancestors (10)

1. [17B](../17b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
