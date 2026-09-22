<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $M(a,b)=\begin{pmatrix}a&b\\0&1\end{pmatrix}$. Direct [matrix multiplication](../../../../../matrix-multiplication.md) gives

$$
M(a,b)M(c,d)=M(ac,ad+b).
$$

Since $a,c\ne0$, the product is again in $G$. [Associativity](../../../../../associative-property.md) is inherited from [matrix multiplication](../../../../../matrix-multiplication.md), the [identity element](../../../../../identity-element.md) is $M(1,0)$, and

$$
M(a,b)^{-1}=M(a^{-1},-b/a)
$$

lies in $G$. These verify all [group axioms](../../../../../group-axioms.md). This is the [Affine group of the complex line](../../../../../affine-group-of-the-complex-line.md), acting by $z\mapsto az+b$.

For the diagonal subset, $M(a,0)M(c,0)=M(ac,0)$, it contains $M(1,0)$, and $M(a,0)^{-1}=M(a^{-1},0)$. Thus $G'$ is a [subgroup](../../../../../subgroup.md). Finally,

$$
f(M(a,b)M(c,d))=M(ac,0)
=M(a,0)M(c,0)=f(M(a,b))f(M(c,d)),
$$

so **$f:G\to G'$ is a surjective [group homomorphism](../../../../../group-homomorphism.md)**.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [9](../../9.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
