<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\widehat\eta$ be the displacement of a material interface and use $[f]_-^+=f_+-f_-$. On each side, the [kinematic boundary condition](../../../../../../kinematic-boundary-condition.md) is

$$
\widehat w_\pm=ik(\overline U_\pm-c)\widehat\eta.
$$

There is one displaced material interface, so its displacement is continuous. Thus **the first jump condition is**

$$
\boxed{\left[\frac{\widehat w}{\overline U-c}\right]_-^+=0.}
$$

In particular, [vertical velocity](../../../../../../vertical-velocity.md) need not be continuous when the background [velocity](../../../../../../velocity.md) jumps.

With no [surface tension](../../../../../../surface-tension.md), [pressure continuity](../../../../../../pressure-continuity.md) applies on the displaced interface, rather than at its undisplaced height. Linearizing gives $[\widehat p+\widehat\eta\,\overline p']_-^+=0$. Since $\overline p'=-g\overline\rho$, this becomes $[\widehat p-g\overline\rho\widehat\eta]_-^+=0$. The horizontal momentum calculation in part (a) gives

$$
\widehat p=\frac{\rho_0}{ik}\bigl[(\overline U-c)\widehat w'-\overline U'\widehat w\bigr].
$$

Substitute this and $\widehat\eta=\widehat w/[ik(\overline U-c)]$ to obtain **the second jump condition**:

$$
\boxed{\left[(\overline U-c)\widehat w'-\overline U'\widehat w-\frac{g\overline\rho}{\rho_0}\frac{\widehat w}{\overline U-c}\right]_-^+=0.}
$$

These [jump conditions for stratified inviscid shear flow](../../../../../../jump-conditions-for-stratified-inviscid-shear-flow.md) use one-sided values of $\overline U'$ and apply to jumps of [mass density](../../../../../../density.md), [vorticity](../../../../../../vorticity.md), or [velocity](../../../../../../velocity.md). If $\overline U$ is continuous, the first condition reduces to continuity of $\widehat w$; a jump of [vorticity](../../../../../../vorticity.md) generally still prevents continuity of $\widehat w'$. This derivation avoids multiplying singular distributional derivatives of a discontinuous [velocity](../../../../../../velocity.md) in the [Taylor–Goldstein equation](../../../../../../taylor-goldstein-equation.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
