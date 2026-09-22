# Hopf normal form

↑ **Parent:** [Hopf bifurcation](hopf-bifurcation.md)

The Hopf normal form is a local [normal form of a dynamical system](normal-form-dynamical-systems.md) on the critical two-dimensional [centre manifold](center-manifold.md). After shifting the [equilibrium point](equilibrium-point-of-a-dynamical-system.md) and changing coordinates, its cubic truncation can be written

$$
\dot z=(\mu+i\omega(\mu))z+(a+ib)z|z|^2,\qquad
\dot r=\mu r+ar^3,\qquad
\dot\theta=\omega(\mu)+br^2,
$$

where $\mu$ is the critical [eigenvalue](eigenvalue.md) [real part](real-part.md), $a=\operatorname{Re}\ell(0)$, $b=\operatorname{Im}\ell(0)$, and $\omega(0)>0$. Smooth parameter dependence of the cubic coefficients and higher-order terms are omitted in this truncation. The real coefficient $a$ controls radial saturation; the imaginary coefficient $b$ changes the [angular frequency](angular-frequency.md) with [amplitude](wave-amplitude.md). This finite-order reduction, rather than literal equality to a cubic equation everywhere, is the meaning of the [Hopf normal form](hopf-normal-form.md) for a general system.[Dmitry Turaev's bifurcation-theory notes, section 3, parameter-dependent complex normal form](https://www.ma.imperial.ac.uk/~dturaev/bif_theory3.pdf)

In the cubic truncation, $r_*^2=-\mu/a$ whenever $\mu a<0$. Substituting into the angular equation gives $\Omega=\omega(\mu)-b\mu/a$. For the full smooth system, the leading [normal form](normal-form-dynamical-systems.md) radius satisfies $r_*^2=-\mu/a+o(|\mu|)$ and the period tends to $2\pi/\omega(0)$. The exact circle and exactly constant [angular frequency](angular-frequency.md) of the special model $a=-1$, $b=0$, $\omega(\mu)=\omega$ are conveniences of that model. In the original coordinates the small [periodic orbit](periodic-orbit.md) need not be a circle. Radial scaling can normalize a nonzero $a$ to $-1$ or $+1$, so $\sqrt{|\mu|}$ is a normalized leading [amplitude](wave-amplitude.md), not a universal physical radius.

<a id="image-computed-radius-branches-and-radial-drift-for-the-two-hopf-criticalities"></a>
![](hopf-criticality-radius-branches.png)

**[Figure 4](#image-computed-radius-branches-and-radial-drift-for-the-two-hopf-criticalities). Computed radius branches and radial drift for the two Hopf criticalities**. The exact cubic [Hopf normal forms](hopf-normal-form.md) $\dot r=\mu r-r^3$ and $\dot r=\mu r+r^3$, with nonzero angular motion understood. The upper [bifurcation diagrams](bifurcation-diagram.md) distinguish attracting solid branches from repelling dashed branches; $r=0$ is an [equilibrium point](equilibrium-point-of-a-dynamical-system.md), while a nonzero constant radius is a [periodic orbit](periodic-orbit.md). Vertical arrows show radial motion at fixed $\mu$. Below, the sign of $\dot r$ shows why the nonzero roots attract or repel. Stability is within the reduced plane. These are original dimensionless calculations, not measured data; continuation away from zero is a property of the chosen cubic equations, not a global prediction of the local [Hopf bifurcation](hopf-bifurcation.md) theorem.

## ↑ Ancestors (6)

1. [Hopf bifurcation](hopf-bifurcation.md)
2. [Bifurcation theory](bifurcation-theory.md)
3. [Dynamical systems](dynamical-systems-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Hopf bifurcation](hopf-bifurcation.md)
- [Hopf normal form](hopf-normal-form.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-58/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-60/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2/7a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/5e/i/solution.md)
- [Subcritical Hopf bifurcation](subcritical-hopf-bifurcation.md)
- [Supercritical Hopf bifurcation](supercritical-hopf-bifurcation.md)
