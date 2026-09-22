<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $G_n(z_1,\ldots,z_n)$ denote the ordered vacuum correlator. Inserting the vacuum-preserving [Möbius transformation](../../../../../mobius-transformation.md) operator and its inverse gives

$$
G_n(z_1,\ldots,z_n)=\prod_i\gamma'(z_i)^{h_i}\,G_n(\gamma(z_1),\ldots,\gamma(z_n)).
$$

For $\gamma(z)=z+\epsilon v(z)$, the three vector fields $v=1,z,z^2$ yield the [global conformal Ward identities for chiral correlators](../../../../../global-conformal-ward-identities-for-chiral-correlators.md)

$$
\sum_i\partial_iG_n=0,\qquad
\sum_i(z_i\partial_i+h_i)G_n=0,\qquad
\sum_i(z_i^2\partial_i+2h_i z_i)G_n=0.
$$

All formulas below concern separated insertion points and a consistent local choice of branches for fractional powers.

For one insertion, the [translation](../../../../../translation-geometry.md) identity makes $G_1$ constant and the [dilation](../../../../../uniform-dilation.md) identity gives $h_1G_1=0$. Thus

$$
\boxed{G_1=C_1\text{ if }h_1=0;\quad G_1=0\text{ if }h_1\ne0}.
$$

For two insertions, [translation](../../../../../translation-geometry.md) invariance gives $G_2=f(z_{12})$, where $z_{ij}=z_i-z_j$. [Dilations](../../../../../uniform-dilation.md) imply $z_{12}f'+(h_1+h_2)f=0$, so $f=C_{12}z_{12}^{-h_1-h_2}$. Substituting into the special conformal identity leaves $(h_1-h_2)z_{12}f=0$. Therefore

$$
\boxed{G_2=\frac{C_{12}}{z_{12}^{2h}},\quad h_1=h_2=h},
$$

with $G_2=0$ when the weights differ.

For three insertions write $G_3=C_{123}z_{12}^{-a}z_{13}^{-b}z_{23}^{-c}$. Under a [Möbius transformation](../../../../../mobius-transformation.md), $\gamma(z_i)-\gamma(z_j)=z_{ij}\sqrt{\gamma'(z_i)\gamma'(z_j)}$ with compatible local branches. The covariance condition therefore fixes

$$
a+b=2h_1,\qquad a+c=2h_2,\qquad b+c=2h_3.
$$

Solving gives

$$
\boxed{G_3=\frac{C_{123}}{z_{12}^{h_1+h_2-h_3}z_{13}^{h_1+h_3-h_2}z_{23}^{h_2+h_3-h_1}}}.
$$

This is the complete solution because [Möbius transformations](../../../../../mobius-transformation.md) act transitively on ordered triples of distinct points: the ratio of any two covariant nonzero solutions has no remaining invariant variable and is constant. **Three-point covariance imposes no equality or triangle inequality among the weights**. Additional fusion rules or other symmetries may force $C_{123}=0$, but none follow from the stated covariance and vacuum assumptions alone.

For more than three generic points, three positions may be fixed by a [Möbius transformation](../../../../../mobius-transformation.md), leaving $n-3$ independent complex [conformal cross-ratios](../../../../../conformal-cross-ratio.md). Correlators consequently have a covariant prefactor multiplied by an arbitrary function of these invariants. For example one convenient four-point form is

$$
G_4=\frac{(z_{24}/z_{14})^{h_1-h_2}(z_{14}/z_{13})^{h_3-h_4}}{z_{12}^{h_1+h_2}z_{34}^{h_3+h_4}}F(\chi),\qquad
\chi=\frac{z_{12}z_{34}}{z_{13}z_{24}}.
$$

The [Möbius invariance of the cross-ratio](../../../../../mobius-invariance-of-the-cross-ratio.md) guarantees covariance for any $F$. Thus **global conformal symmetry fixes one-, two- and three-point functions up to constants, but does not fix higher-point functions**. Their remaining functions encode dynamics.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
