<h1 id="7b/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $H=A-B$. This is a nonzero [Hermitian matrix](../../../../../../hermitian-operator.md). By the [finite-dimensional spectral theorem](../../../../../../finite-dimensional-spectral-theorem.md), it has a unit eigenvector $v$ with a nonzero real eigenvalue $lambda$. Define the rank-one [orthogonal projection matrix](../../../../../../orthogonal-projection-matrix.md)

$$
P=vv^\dagger.
$$

The cyclic property of the [matrix trace](../../../../../../matrix-trace.md) gives

$$
\operatorname{Tr}(PA)-\operatorname{Tr}(PB)
=\operatorname{Tr}(PH)
=\operatorname{Tr}(vv^\dagger H)
=v^\dagger Hv
=\lambda\ne0.
$$

**Hence this $P$ distinguishes $A$ and $B$ through the required traces.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [7B](../../7b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
