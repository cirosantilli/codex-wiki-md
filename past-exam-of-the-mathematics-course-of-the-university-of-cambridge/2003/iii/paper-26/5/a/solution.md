<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [vector field](../../../../../../vector-field.md) on the [sphere](../../../../../../sphere.md) means a tangent [vector field](../../../../../../vector-field.md). For $S^{2m}\subset\mathbb R^{2m+1}$ with $m\ge1$, suppose $V(x)$ were continuous and nowhere zero. Normalize it to $w(x)=V(x)/\|V(x)\|$. Tangency means $\langle x,w(x)\rangle=0$, and both vectors have norm one. Therefore

$$
H(x,t)=\cos(\pi t)x+\sin(\pi t)w(x),\qquad 0\le t\le1,
$$

has squared norm $\cos^2(\pi t)+\sin^2(\pi t)=1$. It defines a [homotopy](../../../../../../homotopy.md) through self-maps of the [sphere](../../../../../../sphere.md) from the identity to the [antipodal map](../../../../../../antipodal-map.md).

The identity has [mapping degree](../../../../../../degree-of-a-continuous-mapping.md) $1$. The antipodal map on $S^n$ has degree $(-1)^{n+1}$: it is the boundary restriction of $-I$ on the oriented $(n+1)$-ball, and this [linear map](../../../../../../linear-map.md) changes [orientation](../../../../../../orientation-of-a-simplex.md) by $\operatorname{sgn}\det(-I)=(-1)^{n+1}$. For $n=2m$ its degree is $-1$. [Homotopy invariance of mapping degree](../../../../../../homotopy-invariance-of-mapping-degree.md) would force $1=-1$, a contradiction. Thus **every continuous tangent field on an even-dimensional [sphere](../../../../../../sphere.md) vanishes somewhere**. For $S^0$ the tangent spaces are zero, so the conclusion holds directly. This proves the [Hairy ball theorem](../../../../../../hairy-ball-theorem.md) using degree, rather than assuming it.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
