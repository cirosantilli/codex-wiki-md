<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The local motion is simple shear with flow direction $z$, gradient direction $r$, and vorticity direction $\theta$. Writing $q=du/dr$, a [second-order fluid](../../../../../../second-order-fluid.md) has first and second normal-stress differences

$$
N_1=\tau_{zz}-\tau_{rr}=\Psi_1q^2,
\qquad
N_2=\tau_{rr}-\tau_{\theta\theta}=\Psi_2q^2.
$$

Up to an isotropic contribution absorbed into pressure, a convenient representation is

$$
\tau_{zz}=(\Psi_1+\Psi_2)q^2,
\qquad \tau_{rr}=\Psi_2q^2,
\qquad \tau_{\theta\theta}=0.
$$

Thus both the flow-direction and gradient-direction normal stresses can be nonzero, while the radial momentum equation becomes

$$
\boxed{\frac{dp}{dr}
=\frac1r\frac{d(r\tau_{rr})}{dr}-\frac{\tau_{\theta\theta}}r
=\frac{\Psi_2}{r}\frac{d}{dr}(rq^2).}
$$

The first normal-stress coefficient affects $\tau_{zz}$ but cancels from radial balance.

In the yielded layer,

$$
q=\frac1\eta\left[
\frac G2\left(\frac{b^2}{r}-r\right)-\sigma_y
\right]>0.
$$

Moreover,

$$
\frac{d}{dr}(rq^2)
=\frac q\eta\left[-\frac G2\left(\frac{b^2}{r}+3r\right)-\sigma_y\right]<0.
$$

**Consequently $dp/dr$ has the sign opposite to $\Psi_2$ and is independent of $\Psi_1$. For the common case $\Psi_2<0$, pressure increases radially outward toward the free surface.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 352](../../../paper-352-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
