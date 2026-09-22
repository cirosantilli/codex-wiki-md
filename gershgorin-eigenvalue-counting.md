# Gershgorin eigenvalue counting

↑ **Parent:** [Gershgorin circle theorem](gershgorin-circle-theorem.md)

Let $C$ be a [connected component](connected-component.md) of the union of the row [Gershgorin discs](gershgorin-disc.md) of an $n\times n$ [matrix](matrix.md). If $C$ comprises $k$ of the indexed [Gershgorin discs](gershgorin-disc.md), then it contains exactly $k$ [eigenvalues](eigenvalue.md), counted with [algebraic multiplicity](algebraic-multiplicity.md). Coincident [disks](disk-mathematics.md) still count separately, once for each row. In particular, a [Gershgorin disc](gershgorin-disc.md) disjoint from all the others contains one simple [eigenvalue](eigenvalue.md). More generally, any union of $k$ indexed [Gershgorin discs](gershgorin-disc.md) disjoint from the remaining $n-k$ contains exactly $k$ [eigenvalues](eigenvalue.md), whether or not that union is connected.[Chi-Kwong Li, Math 408 lecture notes, §6.1, Theorem 6.1.1, p. 48](https://cklixx.people.wm.edu/teaching/math408/408-note.pdf)

The separation is essential: overlapping [Gershgorin discs](gershgorin-disc.md) do not individually promise one [eigenvalue](eigenvalue.md) each. Discs that touch at a boundary point belong to the same [connected component](connected-component.md). For example, the [matrix](matrix.md) $\left(\begin{smallmatrix}2&1&0\\0&2&0\\0&0&8\end{smallmatrix}\right)$ has [Gershgorin discs](gershgorin-disc.md) of radii $1,0,0$ with centres $2,2,8$. The component around $2$ comprises two indexed [disks](disk-mathematics.md) and contains the [eigenvalue](eigenvalue.md) $2$ with [algebraic multiplicity](algebraic-multiplicity.md) two; the isolated point at $8$ contains the remaining [eigenvalue](eigenvalue.md).

For intuition, continuously turn on the off-diagonal entries using the [diagonal matrix](diagonal-matrix.md) $E=\operatorname{diag}(a_{11},\ldots,a_{nn})$ and $A(t)=E+t(A-E)$, $0\leq t\leq1$. At $t=0$ the [eigenvalues](eigenvalue.md) are the disk centres; at every later time the [Gershgorin discs](gershgorin-disc.md) stay inside their final union. The [continuity](continuous-function.md) of the [eigenvalues](eigenvalue.md) as a collection means that no [eigenvalue](eigenvalue.md) can cross a gap between final components. The count gives a useful certificate that an [eigenvalue](eigenvalue.md) cluster is complete.[Gene H. Golub, CME 302, Lecture 2, §6: turning on the off-diagonal entries continuously](https://www.stat.uchicago.edu/~lekheng/courses/302/notes2.pdf)

## ↑ Ancestors (6)

1. [Gershgorin circle theorem](gershgorin-circle-theorem.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Gershgorin circle theorem](gershgorin-circle-theorem.md)
- [Gershgorin disc](gershgorin-disc.md)
