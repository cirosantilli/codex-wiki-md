<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $r=\operatorname{rank}F$ and $s=\operatorname{rank}E$. Around any $p$, choose a [local frame](../../../../../../frame-of-a-vector-bundle.md) $f_1,\ldots,f_r$ of the [vector subbundle](../../../../../../vector-subbundle.md) $F$. Choose additional smooth sections $e_{r+1},\ldots,e_s$ of $E$ which complement these vectors at $p$. They can be obtained by constant-coordinate sections in a [vector bundle trivialization](../../../../../../vector-bundle-trivialization.md). The [determinant](../../../../../../determinant.md) of the resulting frame is nonzero at $p$, hence on a sufficiently small neighborhood. Thus

$$
f_1,\ldots,f_r,e_{r+1},\ldots,e_s
$$

is an adapted [local frame](../../../../../../frame-of-a-vector-bundle.md) of $E$ near $p$.

On the fiberwise quotient, the classes $[e_{r+1}],\ldots,[e_s]$ form a [basis](../../../../../../basis.md). Give the [quotient vector bundle](../../../../../../quotient-vector-bundle.md) its local coordinates by

$$
\sum_{j=r+1}^s a_j[e_j(p)]\longleftrightarrow(p,a_{r+1},\ldots,a_s).
$$

An overlap between adapted frames has a smooth [transition function of a vector bundle](../../../../../../transition-function-of-a-vector-bundle.md) represented by an invertible block upper triangular [matrix](../../../../../../matrix.md),

$$
\begin{pmatrix}A&B\\0&D\end{pmatrix}.
$$

The zero lower-left block expresses that both sets of first $r$ frame vectors span $F$. Its lower-right block $D$ is smooth and invertible. Passing to quotient coordinates removes the upper block, leaving precisely the transition $D$. These lower-right blocks satisfy the cocycle identity because the original transition matrices do. Consequently they define a compatible smooth bundle atlas of rank $s-r$. This proves **$E/F$ is a smooth [vector bundle](../../../../../../vector-bundle.md)**, and its fiberwise quotient map $q:E\to E/F$ is a smooth [vector bundle morphism](../../../../../../vector-bundle-morphism.md). The construction is independent of the adapted frames: any two choices have the same type of compatible transition. The usual quotient topology agrees with this atlas, since in adapted coordinates $q$ is an open linear projection on each [fiber](../../../../../../fiber-of-a-function.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
