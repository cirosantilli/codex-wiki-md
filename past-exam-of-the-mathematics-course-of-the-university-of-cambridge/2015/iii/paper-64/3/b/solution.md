<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an [axisymmetric vertical mode of a shearing sheet](../../../../../../axisymmetric-vertical-mode-of-a-shearing-sheet.md) with real $k\ne0$, the two divergence constraints give $ikv_z=ikb_z=0$. The vertical momentum equation then yields $ikp=0$. Thus **all three amplitudes vanish**:

$$
\boxed{v_z=b_z=p=0.}
$$

Define the magnetic amplitudes $a_i=b_i/\sqrt{4\pi\rho_0}$ and the signed vertical [Alfvén velocity](../../../../../../alfven-velocity.md) $v_A=B_0/\sqrt{4\pi\rho_0}$. Write $A=k^2v_A^2$. The remaining equations for the [normal mode](../../../../../../normal-mode.md) are

$$
\begin{aligned}
\sigma v_x-2\Omega v_y&=-N^2\vartheta+ikv_Aa_x,\\
\sigma v_y+\frac12\Omega v_x&=ikv_Aa_y,\\
\sigma a_x&=ikv_Av_x,\\
\sigma a_y&=-\frac32\Omega a_x+ikv_Av_y,\\
\sigma\vartheta&=v_x.
\end{aligned}
$$

For a growing or oscillatory mode with $\sigma\ne0$, eliminating $a_x,a_y,\vartheta$ gives

$$
(\sigma^2+A+N^2)v_x-2\Omega\sigma v_y=0,
$$



$$
\sigma(\sigma^2+A)v_y+\left(\frac12\Omega\sigma^2-\frac32\Omega A\right)v_x=0.
$$

A nonzero [velocity](../../../../../../velocity.md) requires the determinant to vanish. After removing its factor $\sigma$, **the dynamical [dispersion relation](../../../../../../dispersion-relation.md)** is

$$
\boxed{\sigma^4+(2A+N^2+\Omega^2)\sigma^2+A(A+N^2-3\Omega^2)=0.}
$$

This is the [radially stratified magnetorotational dispersion relation](../../../../../../radially-stratified-magnetorotational-dispersion-relation.md), with $A=k^2B_0^2/(4\pi\rho_0)$. Keeping the original five-amplitude system instead gives characteristic polynomial $\sigma$ times this quartic. There is also a stationary balanced [normal mode](../../../../../../normal-mode.md); division by $\sigma$ excludes it but loses no exponentially growing mode. At $k=0$ the divergence argument for vanishing vertical components does not apply, so that spatially uniform case must be treated separately.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
