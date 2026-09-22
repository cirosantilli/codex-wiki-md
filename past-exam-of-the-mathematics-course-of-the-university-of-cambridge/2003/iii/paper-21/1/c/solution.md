<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $E:y^2=x^3-17x$, the [two-isogeny formula](../../../../../../two-isogeny-formula.md) gives $E':Y^2=X^3+68X$. By the [prime-support bound in two-isogeny descent](../../../../../../prime-support-bound-in-two-isogeny-descent.md), the image of the [two-torsion square-class homomorphism](../../../../../../two-torsion-square-class-homomorphism.md) on $E$ lies in $\{1,-1,17,-17\}$. The identity gives $1$, $T=(0,0)$ gives $-17$, and $P=(-1,4)$ gives $-1$, since $(-1)^3-17(-1)=16$. The image is a [subgroup](../../../../../../subgroup.md) of the [square-class group](../../../../../../square-class-group-of-a-field.md), so their product $17$ occurs as well; explicitly $P+T=(17,68)$. Hence

$$
\alpha(E(\mathbb Q))=\{1,-1,17,-17\}.
$$

On $E'$, a nonzero affine point has $X>0$, because $Y^2=X(X^2+68)$. The only candidate [square classes](../../../../../../square-class.md) are therefore $1,2,17,34$. The identity gives $1$, $T'=(0,0)$ gives $[68]=17$, and $(2,12)$ gives $2$, since $2^3+68\cdot2=144$. Their product $34$ occurs; adding $T'$ gives $(34,-204)$. Thus

$$
\alpha'(E'(\mathbb Q))=\{1,2,17,34\}.
$$

Both images have order four. The [two-isogeny rank formula](../../../../../../square-class-index-formula-for-two-isogeny-descent.md) proves

$$
\boxed{2^r=\frac{4\cdot4}{4}=4,\qquad \operatorname{rank}E(\mathbb Q)=2.}
$$

This is the [rank-two elliptic curve with cubic x cubed minus seventeen x](../../../../../../rank-two-elliptic-curve-with-cubic-x-cubed-minus-seventeen-x.md); all candidate classes are represented, so no unresolved [local-to-global gap in isogeny descent](../../../../../../local-to-global-gap-in-isogeny-descent.md) remains in this computation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
