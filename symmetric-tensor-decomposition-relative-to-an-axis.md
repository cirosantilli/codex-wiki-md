# Symmetric tensor decomposition relative to an axis

↑ **Parent:** [Cartesian second-rank tensor](cartesian-second-rank-tensor.md)

For a real symmetric [Cartesian second-rank tensor](cartesian-second-rank-tensor.md) $T$ and a nonzero [vector](vector.md) $A$, require $B\cdot A=0$ and $C$ symmetric and traceless with $CA=0$. Put $q=A^TA$, $s=A^TTA$, $t=\operatorname{tr}T$, and $P=I-AA^T/q$. The unique decomposition is

$$
\alpha=\frac{t-s/q}{2},\quad\beta=\frac{3s/q-t}{2q},\quad B=\frac{TA}{q}-\frac{sA}{q^2},\quad C=PTP-\alpha P.
$$

The [orthogonal projection](orthogonal-projection.md) $P$ isolates the plane perpendicular to $A$. Splitting $I=P+AA^T/q$ on both sides of $T$ gives its longitudinal, mixed and transverse blocks, proving reconstruction. The transverse [trace](matrix-trace.md) fixes $\alpha$, the longitudinal component fixes $\beta$, and the mixed block fixes $B$, proving uniqueness. The remaining transverse block $C$ has two degrees of freedom. Together $\alpha,\beta,B,C$ carry $1+1+2+2=6$ components, the number in a symmetric three-by-three [matrix](matrix.md).

## ↑ Ancestors (9)

1. [Cartesian second-rank tensor](cartesian-second-rank-tensor.md)
2. [Cartesian tensor](cartesian-tensor.md)
3. [Tensor](tensor.md)
4. [Multilinear algebra](multilinear-algebra-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2/6/solution.md)
