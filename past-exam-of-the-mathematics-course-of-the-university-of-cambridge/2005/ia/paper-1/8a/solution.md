<h1 id="8a/solution">Solution</h1>

↑ **Parent:** [8A](../8a.md)

Use [matrix](../../../../../matrix.md) notation and set $s=\mathbf v^T\mathbf v>0$, $t=\mathbf v^TT\mathbf v$, $\tau=\operatorname{tr}T$. Contracting the proposed decomposition with $\mathbf v$ and taking its [trace](../../../../../matrix-trace.md), using the stipulated transverse and trace conditions, gives

$$
T\mathbf v=(A+Bs)\mathbf v+s\mathbf C,\qquad t=sA+s^2B,\qquad\tau=3A+sB.
$$

These relations determine both scalars and the transverse [vector](../../../../../vector.md) uniquely:

$$
\boxed{A=\frac12\left(\tau-\frac ts\right),\qquad B=\frac{3t-s\tau}{2s^2},\qquad\mathbf C=\frac{T\mathbf v-(t/s)\mathbf v}{s}.}
$$

The last expression obeys $\mathbf C^T\mathbf v=0$ directly.

To construct and check the remaining [symmetric matrix](../../../../../symmetric-matrix.md), use the [orthogonal projection matrix](../../../../../orthogonal-projection-matrix.md) $P=I-\mathbf v\mathbf v^T/s$ onto $\mathbf v^\perp$, and define

$$
\boxed{D=PTP-AP.}
$$

Both terms are symmetric, $D\mathbf v=0$, and

$$
\operatorname{tr}D=\operatorname{tr}(TP)-A\operatorname{tr}P=\tau-\frac ts-2A=0.
$$

Expand $T=(P+Q)T(P+Q)$ with $Q=\mathbf v\mathbf v^T/s$. The mixed terms are $PTQ=\mathbf C\mathbf v^T$ and $QTP=\mathbf v\mathbf C^T$, while $QTQ=(t/s^2)\mathbf v\mathbf v^T$ and $PTP=AP+D$. Consequently

$$
T=AI+\left(\frac t{s^2}-\frac As\right)\mathbf v\mathbf v^T+\mathbf C\mathbf v^T+\mathbf v\mathbf C^T+D,
$$

and the displayed coefficient equals $B$. This proves existence as well as the [axis decomposition of a symmetric matrix](../../../../../axis-decomposition-of-a-symmetric-matrix.md) formulas.

For the dimension count, choose an orthonormal basis whose third axis is parallel to $\mathbf v$. The [vector](../../../../../vector.md) $\mathbf C$ has two transverse components. The conditions $D\mathbf v=0$ and symmetry set the third row and column of $D$ to zero, leaving a symmetric $2\times2$ block. Its zero [trace](../../../../../matrix-trace.md) leaves two independent entries, of the form $\bigl(\begin{smallmatrix}d&e\\e&-d\end{smallmatrix}\bigr)$. Together with the two independent scalars $A,B$, the total is **$1+1+2+2=6$ parameters**, exactly $3(3+1)/2$, the [dimension](../../../../../dimension-vector-space.md) of real symmetric $3\times3$ matrices. The recovery formulas also prove uniqueness, so this is an actual parameterization without redundant degrees of freedom.

## ↑ Ancestors (10)

1. [8A](../8a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
