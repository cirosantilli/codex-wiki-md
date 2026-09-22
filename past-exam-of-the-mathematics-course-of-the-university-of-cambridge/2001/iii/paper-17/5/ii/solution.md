<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $a:X\to Y$ be a [natural transformation](../../../../../../natural-transformation.md) of [categorical presheaves](../../../../../../presheaf-category-theory.md). If every $a_C:X(C)\to Y(C)$ is a [surjective function](../../../../../../surjective-function.md), and $r,s:Y\rightrightarrows Z$ satisfy $ra=sa$, then $r_Ca_C=s_Ca_C$ at every $C$. Surjectivity gives $r_C=s_C$ for all $C$, hence $r=s$. Thus $a$ is an [epimorphism](../../../../../../epimorphism.md).

Conversely suppose $y\in Y(C)$ is outside the image of some $a_C$. Construct the [pushout witness for failure of pointwise surjectivity](../../../../../../pushout-witness-for-failure-of-pointwise-surjectivity.md) explicitly: at each $D$ take

$$
P(D)=\bigl(Y(D)\times\{0,1\}\bigr)/\sim,
\qquad (a_D(x),0)\sim(a_D(x),1).
$$

Restrictions send $[(z,k)]$ to $[(Y(f)z,k)]$; [naturality](../../../../../../naturality.md) of $a$ ensures that every generating identification is respected. Thus $P$ is a [categorical presheaf](../../../../../../presheaf-category-theory.md), and the two inclusions $j_0,j_1:Y\to P$ are [natural transformations](../../../../../../natural-transformation.md) with $j_0a=j_1a$.

All identifications concern the same element $z$ in its two copies, so an element outside the image is never identified with its other copy. Consequently $j_{0,C}(y)\ne j_{1,C}(y)$, proving $a$ is not an [epimorphism](../../../../../../epimorphism.md). Therefore

$$
\boxed{a\text{ is epic}\quad\Longleftrightarrow\quad
\text{every }a_C\text{ is surjective}.}
$$

This is the [pointwise epimorphism in a functor category](../../../../../../pointwise-epimorphism-in-a-functor-category.md) criterion. It requires neither a componentwise choice of preimages nor a natural section.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
