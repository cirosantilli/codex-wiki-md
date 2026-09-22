<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the mostly-plus [Minkowski metric](../../../../../../minkowski-metric.md), with the last spatial coordinate singled out:

$$
\boxed{x^+=\frac{x^{D-1}+x^0}{\sqrt2},\qquad x^-=\frac{x^{D-1}-x^0}{\sqrt2},\qquad x^I=x^I\quad(I=1,\ldots,D-2).}
$$

Then $2dx^+dx^-=(dx^{D-1})^2-(dx^0)^2$, as required. In these [light-cone coordinates](../../../../../../light-cone-coordinates.md), $\partial^+=\partial_-$, $\partial^-=\partial_+$ and $\square_D=2\partial_+\partial_-+\partial_I\partial_I$.

Introduce the [Kalb-Ramond field strength](../../../../../../kalb-ramond-field-strength.md)

$$
H_{pmn}=\partial_pB_{mn}+\partial_mB_{np}+\partial_nB_{pm}.
$$

The field equation is $\partial^pH_{pmn}=0$. Under $\delta B_{mn}=\partial_m\alpha_n-\partial_n\alpha_m$, every second-derivative contribution to $\delta H$ cancels by commutation of derivatives. Thus $H$ and its equation are [gauge-invariant](../../../../../../gauge-invariance.md). This is the differential-form identity $d^2=0$ for the [two-form gauge field](../../../../../../two-form-gauge-field.md) $B$.

To impose [light-cone gauge for a two-form](../../../../../../light-cone-gauge-for-a-two-form.md), first choose $\alpha_-=0$ and

$$
\alpha_m=-\partial_-^{-1}B_{-m}\quad(m=+,I).
$$

This sets $B_{-m}$ to zero. A residual transformation preserving the gauge obeys $\partial_-\alpha_m=\partial_m\alpha_-$. With $\chi=\partial_-^{-1}\alpha_-$, this implies $\alpha_m=\partial_m\chi$, including $m=-$. Such a parameter changes $B$ by zero. Therefore **no nontrivial gauge transformation of $B$ remains** in the sector where $\partial_-$ is invertible. There is still a redundant description of the gauge parameter itself, $\alpha\mapsto\alpha+d\chi$; the excluded $\partial_-$ zero modes would require separate treatment.

The $(-,n)$ field equations now say $\partial_-\partial^pB_{np}=0$, hence $\partial^pB_{np}=0$. For $n=I$ this gives

$$
-\partial_-B_{+I}+\partial^JB_{IJ}=0,
\qquad\boxed{B_{+I}=\partial_-^{-1}\partial^JB_{IJ}.}
$$

For $n=+$, $\partial^IB_{+I}=0$ follows automatically from antisymmetry of $B_{IJ}$. Therefore the independent components and their equation are

$$
\boxed{B_{IJ}=-B_{JI},\qquad\frac{(D-2)(D-3)}2\text{ independent polarizations},\qquad\square_DB_{IJ}=0.}
$$

The remaining equations follow from this wave equation and the reconstructed longitudinal components.

At the first massless level of the [closed bosonic string](../../../../../../closed-string.md), states $\alpha_{-1}^I\widetilde\alpha_{-1}^J|p\rangle$ carry a product of two transverse vector polarizations. Its symmetric traceless, antisymmetric and trace parts are respectively the [graviton](../../../../../../graviton.md), the [Kalb–Ramond field](../../../../../../kalb-ramond-field.md) and the [dilaton](../../../../../../dilaton.md). The antisymmetric part has exactly the polarization count just found.

The [gauge-invariant string coupling to a two-form](../../../../../../gauge-invariant-string-coupling-to-a-two-form.md) uses the pullback of the background [Kalb–Ramond field](../../../../../../kalb-ramond-field.md) to the [string worldsheet](../../../../../../worldsheet.md):

$$
\boxed{I_B=q\int_\Sigma X^*B=\frac q2\int d^2\sigma\,\epsilon^{ab}B_{mn}(X)\partial_aX^m\partial_bX^n.}
$$

Its variation is $q\int_\Sigma d(X^*\alpha)=q\int_{\partial\Sigma}X^*\alpha$, by [Stokes theorem](../../../../../../stokes-theorem.md). It vanishes on a closed [worldsheet](../../../../../../worldsheet.md). For a cylindrical propagation surface it is only an initial/final boundary term, handled by fixed-boundary gauge parameters or the corresponding transformation of external states. Thus the closed string is naturally charged under a [two-form gauge field](../../../../../../two-form-gauge-field.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 306](../../../paper-306-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
