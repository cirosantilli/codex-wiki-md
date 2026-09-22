<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [potential-vorticity gradients in a meridional two-layer current](../../../../../../potential-vorticity-gradients-in-a-meridional-two-layer-current.md) are important here: besides $\bar q_{n,y}=\beta$, one has $\bar q_{1,x}=-FV$ and $\bar q_{2,x}=FV$. They must be retained when linearizing, even though the basic [relative vorticity](../../../../../../relative-vorticity.md) vanishes.

Let $K^2=k^2+l^2$ and $A=K^2+F$. For a [normal mode](../../../../../../normal-mode.md) the [two-layer quasi-geostrophic potential vorticity](../../../../../../two-layer-quasi-geostrophic-potential-vorticity.md) amplitudes are

$$
\widehat q_1=-A\widehat\psi_1+F\widehat\psi_2,\qquad \widehat q_2=F\widehat\psi_1-A\widehat\psi_2.
$$

Because the basic velocities are northward $(V,0)$ in the two layers, their advection frequencies are $\sigma-lV$ and $\sigma$. The uniform forcing has no perturbation, $W'=0$. The linear equations are therefore

$$
(\partial_t+V\partial_y)q'_1+FV\psi'_{1,y}+\beta\psi'_{1,x}=0,
\qquad \partial_tq'_2-FV\psi'_{2,y}+\beta\psi'_{2,x}=0.
$$

In particular, a perturbation's zonal velocity advects the basic interface-induced zonal [potential-vorticity gradient](../../../../../../potential-vorticity-gradient.md). Substitution of the [plane wave](../../../../../../plane-wave.md) gives

$$
\begin{pmatrix}
A(\sigma-lV)+\beta k+FlV&-F(\sigma-lV)\\
-F\sigma&A\sigma+\beta k-FlV
\end{pmatrix}
\begin{pmatrix}\widehat\psi_1\\\widehat\psi_2\end{pmatrix}=0.
$$

A nonzero disturbance exists exactly when the determinant vanishes. The requested relation for [linear stability of a meridional two-layer current](../../../../../../linear-stability-of-a-meridional-two-layer-current.md) is

$$
\boxed{[A(\sigma-lV)+\beta k+FlV][A\sigma+\beta k-FlV]-F^2\sigma(\sigma-lV)=0.}
$$

Equivalently, with $\mathcal B=K^2(K^2+2F)$,

$$
\boxed{\mathcal B\sigma^2+[2A\beta k-\mathcal B lV]\sigma+\beta^2k^2-A\beta klV+FK^2l^2V^2=0.}
$$

Its discriminant is

$$
\Delta_\sigma=4F^2\beta^2k^2+\mathcal B K^2(K^2-2F)l^2V^2.
$$

For $K>0$, exponential [baroclinic instability](../../../../../../baroclinic-instability.md) occurs when this discriminant is negative; otherwise the two frequencies are real. This also displays the stabilizing contribution of the [planetary vorticity](../../../../../../planetary-vorticity.md) gradient when $k\ne0$. As a check, $V=0$ gives the uncoupled [barotropic mode](../../../../../../barotropic-mode.md) and [baroclinic mode](../../../../../../baroclinic-mode.md) frequencies $-\beta k/K^2$ and $-\beta k/(K^2+2F)$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
