<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Retain $\beta=\sqrt{1-V^2/c^2}>0$, but normalize the complex potential as $F=\beta H$, so that $w=\operatorname{Re}F/\beta$. The [Cauchy-Riemann equations](../../../../../../cauchy-riemann-equations.md) give $w_x=\operatorname{Re}F'/\beta$ and $w_y=-\operatorname{Im}F'/\beta$. Since $\partial_{x_2}=\beta\partial_y$, the two stresses satisfy

$$
\boxed{\beta\sigma_{13}-i\sigma_{23}=\mu F'(z).}
$$

Using the same unscaled $H$ from part (a) would instead put an additional $\beta$ on its derivative; the potential normalization matters.

Take the principal branch of $\sqrt z$, with its [branch cut](../../../../../../branch-cut.md) along the negative real axis and positive $\sqrt x$ for $x>0$. Write $Q=F'$. For the antisymmetric crack-opening response, reflection gives $Q^-(s)=-\overline{Q^+(s)}$ on the faces. The prescribed equal face [stress](../../../../../../stress.md) gives $\operatorname{Im}Q^\pm(s)=f(s)/\mu$. Multiplication by the square-root factor converts this face condition to an additive jump. In fact, with $G=\sqrt zQ$ and $r=\sqrt{-s}$,

$$
G^+=irQ^+,\qquad G^-=-irQ^-=ir\overline{Q^+},
\qquad
G^+-G^-=-\frac{2}{\mu}\sqrt{-s}\,f(s).
$$

The [Sokhotski–Plemelj theorem](../../../../../../sokhotski-plemelj-theorem.md) applied to this jump gives

$$
G(z)=-\frac1{\pi i\mu}\int_{-\infty}^0\frac{\sqrt{-s}\,f(s)}{s-z}\,ds+P(z),
$$

where $P$ is entire after imposing the usual finite-energy crack-tip regularity. This is the [Hilbert problem for an antiplane crack](../../../../../../hilbert-problem-for-an-antiplane-crack.md), with the stress-potential phase chosen explicitly above.

For localized face loading with no additional remote loading, the far [displacement](../../../../../../displacement.md) is bounded and the weighted Cauchy transform decays. In particular, for compactly supported loading, $G\to0$ at infinity and [Liouville theorem](../../../../../../liouville-theorem.md) sets $P=0$. The resulting [Cauchy solution for a steadily moving semi-infinite antiplane crack](../../../../../../cauchy-solution-for-a-steadily-moving-semi-infinite-antiplane-crack.md) is

$$
\boxed{F'(z)=-\frac{i}{\pi\mu\sqrt z}
\int_{-\infty}^0\frac{\sqrt{-s}\,f(s)}{z-s}\,ds.}
$$

Integrals and boundary values are understood for loadings with the corresponding convergence and regularity, or as limits of localized loading. The reflection used above is the pure antiplane opening response: reflection with a sign change of [displacement](../../../../../../displacement.md) leaves both prescribed face stresses unchanged, and the usual no-extra-load uniqueness condition eliminates an unforced symmetric addition.

One can check the face stresses directly. Put $I_{\mathrm{pv}}(s)=\operatorname{PV}\int_{-\infty}^0\sqrt{-t}f(t)/(s-t)\,dt$. The Cauchy boundary limits give

$$
Q^+(s)=-\frac{I_{\mathrm{pv}}(s)}{\pi\mu\sqrt{-s}}+\frac{i}{\mu}f(s),
\qquad
Q^-(s)=\frac{I_{\mathrm{pv}}(s)}{\pi\mu\sqrt{-s}}+\frac{i}{\mu}f(s).
$$

Both have $-\mu\operatorname{Im}Q^\pm=-f(s)$, verifying the prescribed [traction](../../../../../../traction.md) and its sign on both faces. The opposite real parts also give the required reflection. Ahead of the tip, the integral is real and $Q$ is purely imaginary, so the bonded line has zero tangential [displacement](../../../../../../displacement.md) gradient and the two halves match.

For $x=x_1-Vt>0$, take $z=x$ in the boxed analytic solution. The ahead-of-tip [stress](../../../../../../stress.md) is

$$
\boxed{\sigma_{23}(x_1,0,t)=\frac1{\pi\sqrt x}
\int_{-\infty}^0\frac{\sqrt{-s}\,f(s)}{x-s}\,ds.}
$$

No $\beta$ appears: **at fixed co-moving position and the specified co-moving face loading, this [stress](../../../../../../stress.md) is independent of the speed**. The [displacement](../../../../../../displacement.md), however, still scales with $1/\beta$, so speed independence does not apply to the whole elastic field. If $\int_{-\infty}^0|f(s)|/\sqrt{-s}\,ds$ is finite, the near-tip [stress](../../../../../../stress.md) is inverse-square-root with coefficient $\pi^{-1}\int f(s)/\sqrt{-s}\,ds$.

The far-field condition is a genuine uniqueness requirement. A [homogeneous stress-intensity field of a semi-infinite antiplane crack](../../../../../../homogeneous-stress-intensity-field-of-a-semi-infinite-antiplane-crack.md) has $Q_h=iC/\sqrt z$, for real $C$. It adds no face [traction](../../../../../../traction.md) but changes the [stress](../../../../../../stress.md) ahead by $-\mu C/\sqrt x$. Although its [stress](../../../../../../stress.md) tends to zero at infinity, its primitive is $2iC\sqrt z$, which gives unbounded remote [displacement](../../../../../../displacement.md) and infinite total [elastic energy](../../../../../../elastic-energy.md). Thus only asking for [stress](../../../../../../stress.md) to vanish at infinity would leave the homogeneous constant undetermined; excluding that added remote stress-intensity loading selects the displayed face-loaded solution. The ordinary inverse-square-root tip singularity itself has finite energy in a bounded neighbourhood and is not being excluded.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
