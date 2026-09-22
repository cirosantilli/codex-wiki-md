<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For fixed $U$, the [categorical coend](../../../../../../coend-of-a-functor.md) on the right is the quotient of $\coprod_W\mathcal C(U,W)\times X(W)$ by the identifications

$$
(fh,x)_V\sim(h,X(f)x)_W\qquad(h:U\to W,\ f:W\to V,\ x\in X(V)).
$$

Define $\Phi_U([h,x])=X(h)x$. This is well defined because the contravariant [functor](../../../../../../functor.md) law gives $X(fh)x=X(h)X(f)x$. Its proposed inverse sends $y\in X(U)$ to $[1_U,y]$. The composite to $X(U)$ is the identity. In the other direction the coend relation, applied with $f=h$ and initial map $1_U$, gives $[h,x]=[1_U,X(h)x]$. Thus the inverse is genuine and

$$
\boxed{X(U)\cong\int^W\mathcal C(U,W)\times X(W).}
$$

For $a:U'\to U$, the coend map replaces $h$ by $ha$; its image is $X(ha)x=X(a)X(h)x$, proving naturality in $U$. A morphism of presheaves acts on $x$ and commutes with every $X(h)$ by naturality, proving naturality in $X$. This is the [density formula for presheaves](../../../../../../density-formula-for-presheaves.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
