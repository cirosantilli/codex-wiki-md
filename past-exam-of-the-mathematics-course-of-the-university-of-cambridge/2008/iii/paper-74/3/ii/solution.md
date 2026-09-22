<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write the total [velocity](../../../../../../velocity.md) as $\mathbf U=\Omega y\widehat{\mathbf x}+\mathbf u$ and the [magnetic field](../../../../../../magnetic-field.md) as $B_0\widehat{\mathbf x}+\mathbf b$. For solenoidal fields the [resistive induction equation](../../../../../../resistive-induction-equation.md) is $(\partial_t+\mathbf U\cdot\nabla)\mathbf B=\mathbf B\cdot\nabla\mathbf U+\eta\nabla^2\mathbf B$. The [first-order smoothing approximation](../../../../../../first-order-smoothing-approximation.md) drops the fluctuating terms $\mathbf b\cdot\nabla\mathbf u-\mathbf u\cdot\nabla\mathbf b$, retaining shear exactly. The uniform field is not stretched by the background shear because $\partial_x(\Omega y)=0$. The other retained stretching terms are $\mathbf b\cdot\nabla(\Omega y\widehat{\mathbf x})=\Omega b_y\widehat{\mathbf x}$ and $B_0\partial_x\mathbf u$. Hence

$$
\partial_t\mathbf b+\Omega y\partial_x\mathbf b=\Omega b_y\widehat{\mathbf x}+B_0\partial_x\mathbf u+\eta\nabla^2\mathbf b.
$$

The same phase cancellation as in part (i), together with $\nabla^2 e^{i\mathbf k\cdot\mathbf x}=-K^2e^{i\mathbf k\cdot\mathbf x}$, proves that a response can be taken as $\operatorname{Re}(\mathbf c(t)e^{i\mathbf k(t)\cdot\mathbf x})$, where

$$
\boxed{\dot{\mathbf c}=\Omega c_y\widehat{\mathbf x}+ik_xB_0\mathbf v-\eta K^2\mathbf c.}
$$

If $\mathbf k\cdot\mathbf c=0$ initially, its derivative is $-\eta K^2\mathbf k\cdot\mathbf c$, so magnetic solenoidality is preserved.

For $j=y,z$ the response equation is $\dot c_j+\eta K^2c_j=ik_xB_0v_j$. Its integrating-factor solution is

$$
c_j(t)=e^{-\eta\int_{t_0}^tK^2ds}c_j(t_0)+ik_xB_0\int_{t_0}^t e^{-\eta\int_\tau^tK^2ds}v_j(\tau)d\tau.
$$

The [velocity](../../../../../../velocity.md) amplitudes and [wavevector](../../../../../../wavevector.md) vary on the shear timescale. In the fast-diffusion limit $\eta(k_x^2+k_y^2)\gg|\Omega|$, and after the free transient, the [integral](../../../../../../integral.md) is concentrated within time $(\eta K^2)^{-1}$ of $t$. Replacing the slowly varying factors there by their current values gives the [quasistatic magnetic response of a helical shearing wave](../../../../../../quasistatic-magnetic-response-of-a-helical-shearing-wave.md):

$$
\boxed{c_y\simeq\frac{ik_xB_0v_y}{\eta K^2},\qquad c_z\simeq\frac{ik_xB_0v_z}{\eta K^2}.}
$$

[Complex conjugation](../../../../../../complex-conjugation.md) introduces a minus sign in $c_j^*$. With precisely the EMF normalization specified in the question,

$$
\mathcal E=\operatorname{Re}\left[-\frac{ik_xB_0}{\eta K^2}(v_yv_z^*-v_zv_y^*)\right]=\boxed{-\frac{B_0H(t)}{\eta K^2}\ \text{to leading order}.}
$$

A literal spatial average of the product of the two real Fourier waves would be half this quantity; no extra factor of $1/2$ belongs in the question's defined $\mathcal E$.

Use $A=k_x^2+k_z^2$ and part (i) to obtain $\mathcal E(t)\simeq-B_0H_0 A/[\eta(A+\Omega^2k_x^2t^2)^2]$. For the time [integral](../../../../../../integral.md), take the driven response without a free magnetic transient and suppose the fast-diffusion approximation holds through the contributing interval, in particular at $t=0$; $\eta k_x^2\gg|\Omega|$ is a sufficient uniform condition. For $\Omega k_x\ne0$, substitute $z=|\Omega k_x|t/\sqrt A$. Since $\int_{-\infty}^{\infty}(1+z^2)^{-2}dz=\pi/2$, this gives

$$
\boxed{\int_{-\infty}^{\infty}\mathcal E(t)dt\simeq-\frac{\pi B_0H_0}{2\eta|\Omega k_x|\sqrt{k_x^2+k_z^2}}.}
$$

The [integral](../../../../../../integral.md) identity follows immediately from $z=\tan\chi$, reducing it to $\int_{-\pi/2}^{\pi/2}\cos^2\chi\,d\chi$. If $k_x=0$, the forcing and $H$ vanish and the driven EMF is zero. If $\Omega=0$ but $H_0\ne0$, the leading EMF is constant rather than time-integrable; the finite [integral](../../../../../../integral.md) relies on nonzero shear.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
