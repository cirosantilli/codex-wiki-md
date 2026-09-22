<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Work in the laboratory frame, with fluid at rest at infinity and the instantaneous [sphere](../../../../../sphere.md) centre at the origin. In the [Unscaled Papkovich–Neuber representation](../../../../../unscaled-papkovich-neuber-representation.md), take the harmonic potentials

$$
\mathbf A=-\frac{3a}{4r}\mathbf V,\qquad\phi=\frac{a^3}{4r^3}(\mathbf V\cdot\mathbf x),\qquad r=|\mathbf x|.
$$

Differentiating the two terms gives the [translating sphere in Stokes flow](../../../../../translating-sphere-in-stokes-flow.md):

$$
\boxed{\mathbf u=\frac{3a}{4r}(I+\mathbf n\mathbf n)\mathbf V+\frac{a^3}{4r^3}(I-3\mathbf n\mathbf n)\mathbf V,\qquad p-p_\infty=\frac{3\mu a}{2r^2}\mathbf V\cdot\mathbf n.}
$$

Here $\mathbf n=\mathbf x/r$. The potentials are harmonic outside the [sphere](../../../../../sphere.md), so they satisfy the [Stokes equations](../../../../../stokes-equation.md). At $r=a$, the two coefficients of $\mathbf n\mathbf n$ cancel and the coefficient of $I$ is one, proving the [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) $\mathbf u=\mathbf V$; the field decays at infinity. Its leading part is a [Stokeslet](../../../../../stokeslet.md) of [force](../../../../../force.md) $6\pi\mu a\mathbf V$ exerted on the fluid.

Let $\widehat{\mathbf z}$ point upwards, $\delta=V_1-V_2$, and $D=a_2V_2-a_1V_1$. Each isolated [sphere](../../../../../sphere.md) moves with [velocity](../../../../../velocity.md) $-V_i\widehat{\mathbf z}$. To leading order its correction is the other's incident [Stokeslet](../../../../../stokeslet.md) [velocity](../../../../../velocity.md):

$$
\dot{\mathbf x}_1=-V_1\widehat{\mathbf z}-\frac{3a_2V_2}{4r}(I+\mathbf n\mathbf n)\widehat{\mathbf z},\qquad\dot{\mathbf x}_2=-V_2\widehat{\mathbf z}-\frac{3a_1V_1}{4r}(I+\mathbf n\mathbf n)\widehat{\mathbf z}.
$$

The [forces](../../../../../force.md) generating these fields are the fixed sedimenting loads, so their leading strengths are set by the isolated speeds. Subtraction yields the [leading interaction of two sedimenting spheres](../../../../../leading-interaction-of-two-sedimenting-spheres.md):

$$
\boxed{\dot{\mathbf r}=-\delta\widehat{\mathbf z}-\frac{3D}{4r}(I+\mathbf n\mathbf n)\widehat{\mathbf z}.}
$$

Since $\widehat{\mathbf z}=\cos\theta\,\widehat{\mathbf r}-\sin\theta\,\widehat{\boldsymbol\theta}$, this reduces to

$$
\boxed{\dot r=-\left(\delta+\frac{3D}{2r}\right)\cos\theta,\qquad r\dot\theta=\left(\delta+\frac{3D}{4r}\right)\sin\theta.}
$$

The stipulated higher-order errors can be appended to both equations; they do not enter this leading calculation.

For the same-sign case, interchange labels if necessary to arrange $\delta>0,D>0$, and put $c=3D/4$. The vertical separation $z=r\cos\theta$ satisfies

$$
\dot z=-\delta-\frac c r(1+\cos^2\theta)\leq-\delta.
$$

If [sphere](../../../../../sphere.md) one is initially above [sphere](../../../../../sphere.md) two, its vertical order reverses; in every case $z\to-\infty$, implying $r\to\infty$. For a noncollinear trajectory there is no collision in the point-force equations. Indeed, divide the two polar equations and integrate:

$$
\frac{\delta r+c}{r(\delta r+2c)}dr=-\cot\theta\,d\theta,\qquad\boxed{r(\delta r+2c)\sin^2\theta=C>0.}
$$

At side-by-side passage, $\theta=\pi/2$, the closest separation is the positive root of $\delta r^2+2cr=C$. Before passage $\dot r<0$ and after passage $\dot r>0$, proving overtaking and unbounded subsequent separation. This [passing invariant for unequal point-force spheres](../../../../../passing-invariant-for-unequal-point-force-spheres.md) describes a physical far-field passage only when the closest separation also greatly exceeds the [sphere](../../../../../sphere.md) radii. Exactly collinear approach instead reaches the near-contact regime, where this leading approximation cannot describe two finite [spheres](../../../../../sphere.md) passing through one another.

For opposite signs, choose $\delta>0,D<0$ and consider the invariant configuration with [sphere](../../../../../sphere.md) one vertically above [sphere](../../../../../sphere.md) two, $\theta=0$. The radial equation is

$$
\dot r=-\delta+\frac{3|D|}{2r}=\delta\left(\frac{r_*}{r}-1\right),\qquad\boxed{r_*=-\frac{3D}{2\delta}.}
$$

If $r>r_*$, separation decreases; if $r<r_*$, it increases. Thus it approaches this [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) along the vertical line. [Linearization](../../../../../linearization.md) gives $\dot{\delta r}=-(\delta/r_*)\delta r$. But a small tilt obeys $\dot\theta=(\delta/(2r_*))\theta$, so the [vertical bound pair in the point-force sedimentation model](../../../../../vertical-bound-pair-in-the-point-force-sedimentation-model.md) is stable only against vertical perturbations and is a saddle in the full separation dynamics. The opposite vertical orientation has the reversed stability. Reversing gravity reverses both $\delta$ and $D$, leaves $r_*$ unchanged, and reverses every trajectory; radial attraction becomes repulsion. This is fully consistent with [kinematic reversibility of Stokes flow](../../../../../kinematic-reversibility-of-stokes-flow.md).

There is an important restriction in the printed data. Its hierarchy $|D|\ll(a_1+a_2)|\delta|$ implies $r_*\ll a_1+a_2$, so the proposed [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) would overlap the physical [spheres](../../../../../sphere.md) and lie outside the well-separated approximation. **With that hierarchy there is no justified physical far-field bound pair.** The intended far-field [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) instead requires the first inequality reversed, $|D|\gg(a_1+a_2)|\delta|$. The formal [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) and its vertical stability above show the intended mechanism, while also identifying the missing validity and transverse-stability qualifications.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 86](../../paper-86-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
