<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Ignore the zero-area boundary sets where a reciprocal or its digit is undefined, and put $a=\lfloor1/x\rfloor$. On this digit branch the [natural extension of the continued-fraction Gauss map](../../../../../../natural-extension-of-the-continued-fraction-gauss-map.md) has inverse

$$
x=\frac1{a+x'},\qquad y=\frac1{y'}-a,
\qquad a=\left\lfloor\frac1{y'}\right\rfloor.
$$

The images are the disjoint horizontal strips $1/(a+1)<y'<1/a$, covering the square almost everywhere. Thus the branch calculation proves global invariance without an extra sum over overlapping branches.

Its [Jacobian determinant](../../../../../../jacobian-determinant.md) has magnitude $J=[x^2(a+y)^2]^{-1}$. Since

$$
1+x'y'=\frac{a+y+1/x-a}{a+y}=\frac{1+xy}{x(a+y)},
$$

the transformed density satisfies

$$
P(x',y')J=\frac1{(\log2)(1+x'y')^2}\frac1{x^2(a+y)^2}=P(x,y).
$$

The [change of variables formula](../../../../../../change-of-variables-formula.md) therefore proves invariance. Normalization follows from

$$
\int_0^1\frac{dy}{(1+xy)^2}=\frac1{1+x},\qquad
\int_0^1\frac{dx}{(\log2)(1+x)}=1.
$$

Projecting onto the first coordinate commutes with the [Gauss continued-fraction map](../../../../../../gauss-continued-fraction-map.md), so its invariant marginal is the [Gauss measure](../../../../../../gauss-measure.md):

$$
\boxed{p_G(x)=\frac1{(\log2)(1+x)},\quad 0<x<1.}
$$

One may also check it directly. The inverse branches $h_a(x)=(a+x)^{-1}$ give

$$
\sum_{a\geq1}p_G(h_a(x))|h_a'(x)|
=\frac1{\log2}\sum_{a\geq1}\frac1{(a+x)(a+x+1)}=p_G(x),
$$

where the last sum telescopes. Values assigned at the exceptional boundary points do not affect the absolutely continuous [invariant measure](../../../../../../invariant-measure.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
