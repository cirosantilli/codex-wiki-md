# Electric flux

↑ **Parent:** [Electric field](electric-field-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Electric_flux)

[Electric flux](electric-flux.md) measures how much [electric field](electric-field-split.md) crosses a chosen [oriented surface](oriented-surface.md), with a sign distinguishing the two crossing directions. A strong [electric field](electric-field-split.md) running along a surface contributes nothing to its [electric flux](electric-flux.md): only the [normal component](normal-component.md) counts. This lets [Gauss's law](gauss-s-law.md) turn a potentially complicated [electric field](electric-field-split.md) into one number recording the net enclosed [electric charge](electric-charge-split.md).

For a surface $S$ with chosen [unit normal](unit-normal.md) $\mathbf n$, the [electric flux](electric-flux.md) is the [surface integral](surface-integral.md)

$$
\Phi_E(S)=\int_S\mathbf E\cdot\mathbf n\,dA=\int_S\mathbf E\cdot d\mathbf S,\qquad d\mathbf S=\mathbf n\,dA.
$$

Here $dA$ is positive [surface area](surface-area.md), while $d\mathbf S$ is the [vector area element](vector-area-element.md). The [dot product](dot-product.md) makes [electric flux](electric-flux.md) a signed [scalar](scalar.md), rather than a [vector](vector.md) like the [electric field](electric-field-split.md). Its [SI](international-system-of-units.md) unit is $\mathrm{N\,m^2/C}$: [electric field](electric-field-split.md) measured using the [newton](newton-unit.md) per [coulomb](coulomb.md), multiplied by [surface area](surface-area.md) in square metres. Reversing the [orientation of a surface](orientation-of-a-surface.md) replaces $\mathbf n$ by $-\mathbf n$ and reverses the [electric flux](electric-flux.md). Calling it [electric flux](electric-flux.md) does not imply that [electric charge](electric-charge-split.md) is moving through the surface. [Feynman lectures II.3, §3–2: flux of a vector field](https://www.feynmanlectures.caltech.edu/II_03.html#Ch3-S2).

For an open patch in a [plane](plane.md), with [surface area](surface-area.md) $A$ and a constant [electric field](electric-field-split.md), the [unit normal](unit-normal.md) is constant and the [surface integral](surface-integral.md) simplifies to

$$
\Phi_E=\mathbf E\cdot(A\mathbf n)=EA\cos\theta,\qquad E=|\mathbf E|.
$$

The [angle](angle.md) $\theta$ is between the [electric field](electric-field-split.md) and the chosen [unit normal](unit-normal.md), not between the [electric field](electric-field-split.md) and the [plane](plane.md). The [cosine](cosine.md) describes the signed projected [surface area](surface-area.md) seen by the [electric field](electric-field-split.md). Thus [electric flux](electric-flux.md) is positive for $0\leq\theta<90^\circ$, zero at $90^\circ$, and negative for $90^\circ<\theta\leq180^\circ$. [Ling, Sanny and Moebs, University Physics II, §6.1: electric flux](https://openstax.org/books/university-physics-volume-2/pages/6-1-electric-flux).

For example, take $E=100\,\mathrm{N/C}$ and $A=0.02\,\mathrm{m^2}$, so $EA=2\,\mathrm{N\,m^2/C}$. Three choices of [angle](angle.md) give

$$
\begin{aligned}
\Phi_E(0^\circ)&=2\cos0^\circ=2\,\mathrm{N\,m^2/C},\\
\Phi_E(60^\circ)&=2\cos60^\circ=1\,\mathrm{N\,m^2/C},\\
\Phi_E(120^\circ)&=2\cos120^\circ=-1\,\mathrm{N\,m^2/C}.
\end{aligned}
$$

Keeping the $60^\circ$ patch fixed and reversing its [unit normal](unit-normal.md) gives $120^\circ$ and changes $+1$ to $-1\,\mathrm{N\,m^2/C}$. The [electric field](electric-field-split.md) and physical patch have not changed. If the [electric field](electric-field-split.md) is instead tangent to the patch, its [dot product](dot-product.md) with the [unit normal](unit-normal.md) vanishes: [electric flux](electric-flux.md) is zero even though $E=100\,\mathrm{N/C}$.

<a id="image-three-open-patches-in-a-plane-in-a-constant-electric-field-the-angle-to-the-chosen-unit-normal-gives-electric-fluxes-of-2-1-and-minus-1-newton-square-metres-per-coulomb"></a>
![](open-surface-electric-flux.png)

**[Figure 1](#image-three-open-patches-in-a-plane-in-a-constant-electric-field-the-angle-to-the-chosen-unit-normal-gives-electric-fluxes-of-2-1-and-minus-1-newton-square-metres-per-coulomb). Three open patches in a plane in a constant electric field: the angle to the chosen unit normal gives electric fluxes of 2, 1 and minus 1 newton square metres per coulomb**.

For a [closed surface](closed-surface.md) enclosing a volume $V$, choose the outward [unit normal](unit-normal.md). [Gauss's law](gauss-s-law.md) gives

$$
\Phi_E(\partial V)=\oint_{\partial V}\mathbf E\cdot\mathbf n\,dA=\frac{Q_{\mathrm{enclosed}}}{\varepsilon_0}.
$$

Here $\varepsilon_0$ is the [vacuum permittivity](vacuum-permittivity.md), and $Q_{\mathrm{enclosed}}$ is the signed total [electric charge](electric-charge-split.md) inside. The [electric field](electric-field-split.md) in the [surface integral](surface-integral.md) includes all sources, including external [electric charges](electric-charge-split.md). Assume no ideal [point charge](point-charge.md) lies on the integration surface. Zero enclosed [electric charge](electric-charge-split.md) implies zero total [electric flux](electric-flux.md); it does **not** imply zero [electric field](electric-field-split.md) everywhere on the [closed surface](closed-surface.md) or inside it. Positive and negative contributions to the [surface integral](surface-integral.md) can cancel. [Ling, Sanny and Moebs, University Physics II, §6.2: outward flux and enclosed charge](https://openstax.org/books/university-physics-volume-2/pages/6-2-explaining-gausss-law).

To see the cancellation with sources inside, place [point charges](point-charge.md) $+q$ at $(-a,0,0)$ and $-q$ at $(a,0,0)$, where $q>0$, $a=0.30\,\mathrm m$, and both lie inside the [sphere](sphere.md) of radius $R=1\,\mathrm m$ centered at the origin. This separated pair has the [electric dipole](electric-dipole.md) geometry. Its enclosed [electric charge](electric-charge-split.md) is $q-q=0$, so its total outward [electric flux](electric-flux.md) is zero. At the point $P=(0,0,R)$ on the [sphere](sphere.md), [Coulomb's law](coulomb-s-law.md) and the [superposition principle](superposition-principle.md) give the individual [electric fields](electric-field-split.md)

$$
\mathbf E_+(P)=\frac{kq(a,0,R)}{(R^2+a^2)^{3/2}},\qquad
\mathbf E_-(P)=\frac{kq(a,0,-R)}{(R^2+a^2)^{3/2}},\qquad k=\frac{1}{4\pi\varepsilon_0}.
$$

The $z$ components cancel and the positive $x$ components add:

$$
\mathbf E(P)=\frac{2kqa}{(R^2+a^2)^{3/2}}\widehat{\mathbf x}\approx0.527244\frac{kq}{R^2}\widehat{\mathbf x}\ne\mathbf0.
$$

For the stipulated approximation $k=8.99\times10^9\,\mathrm{N\,m^2/C^2}$ and $q=1\,\mathrm{nC}$, this is about $4.740\,\mathrm{N/C}$ along positive $x$. At $P$, the outward [unit normal](unit-normal.md) is $\widehat{\mathbf z}$, so this nonzero [electric field](electric-field-split.md) is tangent to the [sphere](sphere.md). At other points of the [sphere](sphere.md), its [normal component](normal-component.md) can be positive or negative. The source-field formula applies away from the two [point charges](point-charge.md), where the [electric field](electric-field-split.md) has zero [divergence](divergence.md); it is singular at the sources. [Feynman lectures II.4, §§4–1 and 4–2: electrostatic sources and superposition](https://www.feynmanlectures.caltech.edu/II_04.html#Ch4-S2).

<a id="image-cross-section-of-the-three-dimensional-electric-field-of-two-opposite-point-charges-inside-a-unit-radius-sphere-zero-total-electric-flux-coexists-with-a-nonzero-tangential-electric-field-at-the-top"></a>
![](zero-net-flux-nonzero-field.png)

**[Figure 2](#image-cross-section-of-the-three-dimensional-electric-field-of-two-opposite-point-charges-inside-a-unit-radius-sphere-zero-total-electric-flux-coexists-with-a-nonzero-tangential-electric-field-at-the-top). Cross-section of the three-dimensional electric field of two opposite point charges inside a unit-radius sphere: zero total electric flux coexists with a nonzero tangential electric field at the top**.

The diagram shows [streamlines](streamline.md) of the three-dimensional [electric field](electric-field-split.md) in the section $y=0$. The circle is a cross-section of the [sphere](sphere.md), not the integration surface: [Gauss's law](gauss-s-law.md) uses the entire three-dimensional [surface integral](surface-integral.md). A two-dimensional [line integral](line-integral.md) of outward field around that circle would be a different quantity, with units $\mathrm{N\,m/C}$ rather than the [electric flux](electric-flux.md) units $\mathrm{N\,m^2/C}$.

## ↑ Ancestors (5)

1. [Electric field](electric-field-split.md)
2. [Electromagnetism](electromagnetism-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (17)

- [Conductor in electrostatic equilibrium](conductor-in-electrostatic-equilibrium.md)
- [Coulomb's law](coulomb-s-law.md)
- [Electric flux](electric-flux.md)
- [Electrostatic boundary conditions at a conductor](electrostatic-boundary-conditions-at-a-conductor.md)
- [Faraday's ice pail experiment](faraday-s-ice-pail-experiment.md)
- [Fringing field of a capacitor](fringing-field-of-a-capacitor.md)
- [Gauss's law](gauss-s-law.md)
- [Gaussian surface](gaussian-surface.md)
- [Maxwell equations](maxwell-equations-split.md)
- [Net charge from the asymptotic radial electric field](net-charge-from-the-asymptotic-radial-electric-field.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-59/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/6a/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1/section-b/b6/a/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-1/section-a/a2/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2013/paper-2/section-b/b6/a/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1/section-e/e15/d/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/section-e/15/d/solution.md)
