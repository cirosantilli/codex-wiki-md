<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $\delta F=\epsilon\{F,\varphi\}$ with the canonical [Poisson bracket](../../../../../../poisson-bracket.md). The [first-class constraint](../../../../../../first-class-constraint.md) generates

$$
\boxed{\delta x^m=\epsilon p^m,\qquad \delta p_m=0,\qquad \delta e=\dot\epsilon.}
$$

Indeed the variation of the [relativistic particle phase-space action](../../../../../../relativistic-particle-phase-space-action.md) is

$$
\delta I=\int dt\,\left\{\frac12\frac{d}{dt}
[\epsilon(p^2-M^2)]+(\dot\epsilon-\delta e)\varphi\right\}.
$$

The transformation is therefore a [gauge invariance](../../../../../../gauge-invariance.md) when its parameter vanishes at the time endpoints, or suitable boundary conditions remove the total derivative.

On a fixed interval of parameter length $\Delta t$, the [proper-time modulus](../../../../../../proper-time-modulus.md)

$$
s=\frac1{\Delta t}\int_{t_i}^{t_f}e(t)\,dt
$$

is unchanged by these [gauge transformations](../../../../../../gauge-transformation.md). Choosing $\epsilon(t)=\int_{t_i}^{t}(s-e(u))\,du$ sets $e+\delta e=s$, with $\epsilon(t_i)=\epsilon(t_f)=0$. Thus **the nonconstant part of the [worldline einbein](../../../../../../worldline-einbein.md) can be fixed, but its constant modulus must still be integrated over**. Fixing $e=1$ as well would remove inequivalent values of the [proper-time modulus](../../../../../../proper-time-modulus.md); it is legitimate only if the parameter interval is allowed to vary instead. The name proper-time modulus refers to the Schwinger proper-time parameter; after eliminating $p$, the geometric proper length for a massive on-shell trajectory is $M\int e\,dt$ in this normalization.

For the [gauge fixing](../../../../../../gauge-fixing.md) functional $F=e-s$, its variation is $\delta F=\dot\epsilon$. The [Faddeev-Popov determinant](../../../../../../faddeev-popov-determinant.md) is consequently

$$
\Delta_{\mathrm{FP}}=\det\bigl[\partial_t\delta(t-t')\bigr].
$$

The [Grassmann Gaussian integral](../../../../../../grassmann-gaussian-integral.md) represents this determinant using anticommuting [Faddeev-Popov ghost fields](../../../../../../faddeev-popov-ghost.md) $b,c$:

$$
\boxed{I_{\mathrm{FP}}=i\int dt\,b\dot c,\qquad
\int\mathcal Db\,\mathcal Dc\,e^{iI_{\mathrm{FP}}}\ \propto\ \det(\partial_t).}
$$

The phase and normalization of the determinant depend on the measure convention. Its domain carries the chosen boundary conditions: on an interval the constant modulus is excluded from the gauge-fixed directions, and on a periodic [worldline](../../../../../../world-line.md) the constant ghost [zero mode in field theory](../../../../../../zero-mode-in-field-theory.md) is removed with the residual gauge volume treated separately. A bare determinant with such zero modes left in would vanish.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 306](../../../paper-306-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
