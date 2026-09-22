<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the polynomial graded [ring](../../../../../../ring.md) $R[x_0,x_1,x_2,x_3]$, as in the PDF; the doubled brackets in the converted TeX are an OCR error. Let $I$ denote the homogeneous defining [ideal](../../../../../../ideal.md). The four cubic coordinates in the proposed map never vanish simultaneously on $\mathbb P_F^1$, since $y_0^3$ and $y_1^3$ already have that property. Substitution makes each generator of $I$ zero, so they define a morphism into the generic fibre.

The two standard opens $D_+(x_0)$ and $D_+(x_3)$ cover $X$. Indeed, a homogeneous prime containing $x_0,x_3$ contains $x_2$ by $x_0x_3^2=x_2^3$, and then contains $x_1$ by $x_1^2=\pi^2x_0x_2$. Such a prime contains the irrelevant [ideal](../../../../../../ideal.md) and gives no point of Proj.

On $D_+(x_0)$ put $a=x_1/x_0$, $b=x_2/x_0$, $c=x_3/x_0$. Over $F$, where $\pi$ is invertible, the equations give

$$
a=\pi t,\qquad b=t^2,\qquad c=t^3,\qquad t=a/\pi.
$$

Thus the generic-fibre chart is exactly $\operatorname{Spec}F[t]$. The proposed map restricts to this [isomorphism](../../../../../../isomorphism.md) with $t=y_1/y_0$. On $D_+(x_3)$ put $s=x_2/x_3$. The equations give

$$
x_0/x_3=s^3,\qquad x_1/x_3=\pi s^2,
$$

so this chart is $\operatorname{Spec}F[s]$, and the map has $s=y_0/y_1$. On the overlap $s=t^{-1}$. These are the standard two charts of the [projective line](../../../../../../projective-line.md), proving the scheme-level [isomorphism](../../../../../../isomorphism.md)

$$
\boxed{\mathbb P_F^1\xrightarrow{\sim}X_F.}
$$

Equivalently, rescaling $x_1$ by $\pi^{-1}$ gives the usual [twisted cubic](../../../../../../twisted-cubic.md). The chart proof also shows that the extra cubic relation introduces no additional generic-fibre [scheme](../../../../../../scheme.md) structure.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 89](../../../paper-89-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
