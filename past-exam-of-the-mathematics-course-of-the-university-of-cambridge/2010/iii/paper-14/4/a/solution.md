<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [coorientation](../../../../../../coorientation.md) gives a globally nonvanishing $C^2$ [one-form](../../../../../../one-form.md) $\zeta$ with $E=\ker\zeta$. For tangent fields $A,B$ in the [integrable distribution](../../../../../../integrable-distribution.md),

$$
d\zeta(A,B)=-\zeta([A,B])=0,
$$

since integrability makes their bracket tangent to $E$. Thus $\zeta\wedge d\zeta=0$. Choose a transverse field $Y$ with $\zeta(Y)=1$. The $C^1$ [one-form](../../../../../../one-form.md) $\eta=-\iota_Yd\zeta$ then satisfies $d\zeta=\eta\wedge\zeta$, as is checked on $E$ and $Y$.

The [Godbillon-Vey invariant](../../../../../../godbillon-vey-invariant.md) in the unnormalized convention is

$$
\boxed{\mathrm{gv}(E)=\int_N\eta\wedge d\eta}.
$$

The three-form is continuous at the specified regularity, so its integral is defined. We prove independence of both choices by producing exact differences with $C^1$ primitives, allowing ordinary [Stokes theorem](../../../../../../stokes-theorem.md).

First, for a fixed $\zeta$, another admissible auxiliary form has the form $\eta' =\eta+a\zeta$. From $d^2\zeta=0$ and $d\zeta=\eta\wedge\zeta$, one gets $d\eta\wedge\zeta=0$. Expanding the two three-forms, using this relation and $\zeta\wedge d\zeta=0$, gives

$$
\begin{aligned}
\eta'\wedge d\eta'-\eta\wedge d\eta
&=\eta\wedge da\wedge\zeta\\
&=-da\wedge d\zeta=-d(a\,d\zeta).
\end{aligned}
$$

Its integral on the closed manifold vanishes.

Next any other defining form is $\zeta'=h\zeta$ with $h$ nowhere zero. Let $g=\log|h|$. Then

$$
d\zeta'=(\eta+dg)\wedge\zeta',
$$

so one may use $\eta_0'=\eta+dg$. Its three-form differs by

$$
\eta_0'\wedge d\eta_0'-\eta\wedge d\eta
=dg\wedge d\eta=d(-dg\wedge\eta).
$$

Again the difference integrates to zero; any subsequent auxiliary choice is handled by the first calculation. This includes reversing the chosen [coorientation](../../../../../../coorientation.md), since $h$ can be negative. Thus the invariant, and the corresponding [de Rham cohomology](../../../../../../de-rham-cohomology.md) class, depends only on the oriented manifold and the [foliation](../../../../../../foliation.md) defined by $E$. Reversing the orientation of $N$, unlike reversing the [coorientation](../../../../../../coorientation.md) of $E$, changes the sign of its numerical value.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
