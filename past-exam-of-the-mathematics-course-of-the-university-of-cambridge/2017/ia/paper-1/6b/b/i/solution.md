<h1 id="6b/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

If $p=m\times n$, then $n^Tp=0$, and hence $Bp=p$. Also $Bm=m$ because $m\perp n$. Thus $p$ and $m$ are linearly independent eigenvectors with eigenvalue one.

For every vector $v$,

$$
(B-I)v=m(n^Tv),
$$

so $B-I$ is nonzero but has square zero:

$$
(B-I)^2=mn^Tmn^T=0.
$$

Consequently all three eigenvalues are one. The eigenspace is

$$
\ker(B-I)=\{v:n^Tv=0\}=n^\perp,
$$

which has dimension two. It cannot supply three linearly independent eigenvectors, so

$$
\boxed{B\text{ has eigenvalues }1,1,1\text{ and is not diagonalizable}.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [6B](../../../6b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ia](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
