<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose the smooth [fiber metric](../../../../../../fiber-metric.md) supplied by part (a), and let $P_p:E_p\to F_p$ be [orthogonal projection](../../../../../../orthogonal-projection.md). These projections vary smoothly. Indeed, in a [local frame](../../../../../../frame-of-a-vector-bundle.md) of $E$ write its metric as a [positive-definite](../../../../../../positive-definite-bilinear-form.md) [matrix](../../../../../../matrix.md) $G(p)$, and let the columns of $A(p)$ be a frame of $F$. Then

$$
P=A(A^tGA)^{-1}A^tG.
$$

The [matrix](../../../../../../matrix.md) $A^tGA$ is positive definite, so its inverse is smooth. This formula proves smoothness of the intrinsic projections in every chart. It also gives $P^2=P$ and $\operatorname{im}P=F$.

The [orthogonal complement](../../../../../../orthogonal-complement.md) $F^\perp=\ker P$ is a smooth [vector subbundle](../../../../../../vector-subbundle.md): applying $I-P$ to a complement frame gives a frame of its [fibers](../../../../../../fiber-of-a-function.md), of constant rank $s-r$, after shrinking the chart. Fiberwise,

$$
E=F\oplus F^\perp,
$$

and the restriction $q|_{F^\perp}:F^\perp\to E/F$ is a smooth fiberwise bijective [vector bundle morphism](../../../../../../vector-bundle-morphism.md). In [local frames](../../../../../../frame-of-a-vector-bundle.md) its [matrix](../../../../../../matrix.md) is invertible, with smooth inverse, so it is a [vector bundle isomorphism](../../../../../../vector-bundle-isomorphism.md).

More explicitly, the desired [orthogonal splitting of a vector subbundle](../../../../../../orthogonal-splitting-of-a-vector-subbundle.md) is

$$
\boxed{\Psi:E\longrightarrow F\oplus(E/F),\qquad \Psi(v)=(Pv,[v]).}
$$

Its inverse is $(f,[v])\mapsto f+(I-P)v$. Replacing $v$ by $v+w$ with $w\in F_p$ leaves $(I-P)v$ unchanged, so the inverse is well-defined. Both maps are smooth and linear on [fibers](../../../../../../fiber-of-a-function.md), and their compositions are identities. The splitting exists globally but depends on the chosen [fiber metric](../../../../../../fiber-metric.md).

## ↑ Ancestors (11)

1. [C](../c.md)
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
