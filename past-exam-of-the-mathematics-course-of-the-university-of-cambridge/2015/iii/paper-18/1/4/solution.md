<h1 id="1/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the complex-bilinear extension of the [Nijenhuis tensor](../../../../../../nijenhuis-tensor.md) expression to complex [vector fields](../../../../../../vector-field.md). If $U,V\in T^{1,0}X$, then $JU=iU$ and $JV=iV$, so

$$
N(U,V)=-4[U,V]-4iJ[U,V]=-8[U,V]^{0,1}.
$$

For $U,V\in T^{0,1}X$, the same substitution with $-i$ gives $N(U,V)=-8[U,V]^{1,0}$. For inputs of opposite types, the two leading [Lie brackets](../../../../../../lie-bracket.md) cancel, as do the two terms involving $J$, so $N(U,V)=0$. Applying the [type decomposition of the complexified tangent bundle](../../../../../../type-decomposition-of-the-complexified-tangent-bundle.md) to both inputs consequently gives

$$
\boxed{N(\alpha,\beta)=-8[\alpha',\beta']''-8[\alpha'',\beta'']',\qquad
N(\alpha,\beta)''=-8[\alpha',\beta']''.}
$$

Thus $N=0$ precisely when the [Lie bracket](../../../../../../lie-bracket.md) of any two sections of either [eigenbundle](../../../../../../eigenbundle.md) remains in that same [eigenbundle](../../../../../../eigenbundle.md). In other words, **$N=0$ if and only if both tangent-type distributions are [involutive distributions](../../../../../../involutive-distribution.md)**. This proves the equivalence directly and does not assume that an arbitrary [almost complex structure](../../../../../../almost-complex-manifold.md) already has holomorphic coordinates.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [1](../../1.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
