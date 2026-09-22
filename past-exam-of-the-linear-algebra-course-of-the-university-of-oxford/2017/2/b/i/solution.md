<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [annihilator of a vector subspace](../../../../../annihilator-of-a-vector-subspace.md) is

$$
U^\circ=\{\phi\in V':\phi(u)=0\text{ for every }u\in U\}.
$$

Choose a [basis](../../../../../basis.md) $e_1,\ldots,e_r$ of $U$ and extend it to a [basis](../../../../../basis.md) $e_1,\ldots,e_d$ of $V$. In the [dual basis](../../../../../dual-basis.md), precisely $f_{r+1},\ldots,f_d$ span $U^\circ$. Therefore

$$
\boxed{\dim U^\circ=\dim V-\dim U.}
$$

The canonical restriction [linear transformation](../../../../../linear-map.md)

$$
\rho:V'\longrightarrow U',\qquad \rho(\phi)=\phi|_U
$$

has [kernel of a linear map](../../../../../kernel-of-a-linear-map-split.md) $U^\circ$. It is surjective: extend any [linear functional](../../../../../linear-functional.md) on $U$ by assigning arbitrary values, for instance zero, to the additional [basis](../../../../../basis.md) vectors. The [First isomorphism theorem for vector spaces](../../../../../first-isomorphism-theorem-for-vector-spaces.md) gives the explicit [linear isomorphism](../../../../../linear-isomorphism.md)

$$
\boxed{V'/U^\circ\ \longrightarrow U',\qquad
\phi+U^\circ\longmapsto\phi|_U.}
$$

It is natural because the displayed map itself makes no [basis](../../../../../basis.md) choice; a [basis](../../../../../basis.md) was used only to prove surjectivity. In particular, $U'$ is canonically a [quotient vector space](../../../../../quotient-vector-space.md) of $V'$, rather than canonically a subspace of $V'$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the linear algebra course of the University of Oxford](../../../../split.md)
6. [Linear algebra course of the University of Oxford](../../../../../linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
