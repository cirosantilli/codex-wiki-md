<h1 id="5/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**False.** Take $M=S^4$ and $N=S^3$. Both are closed oriented [simply connected](../../../../../../simply-connected-space.md) manifolds and $4>3$. A cohomological obstruction rules out even a topological [fiber bundle](../../../../../../fiber-bundle-split.md).

Suppose a [fiber bundle](../../../../../../fiber-bundle-split.md) $F\to S^4\to S^3$ existed. The [long exact sequence of homotopy groups of a fibration](../../../../../../long-exact-sequence-of-homotopy-groups-of-a-fibration.md), including its component terms, makes $F$ path-connected. A local trivialization over a small open ball in $S^3$ identifies its preimage, an open subset of $S^4$, with $F\times B^3$. Projection onto $F\times\{0\}$ gives a retraction. An open smooth four-manifold has the homotopy type of a [CW complex](../../../../../../cw-complex.md) of dimension at most four, so its rational cohomology vanishes in degrees above four. A retract's cohomology injects into that of the ambient space. Therefore

$$
H^j(F;\mathbb Q)=0\qquad(j>4).
$$

Use the multiplicative [cohomological Serre spectral sequence](../../../../../../cohomological-serre-spectral-sequence.md) with rational coefficients. Since $S^3$ is simply connected, there is no nontrivial coefficient action, and only columns zero and three occur on $E_2$. Thus $E_3=E_2$, and the only possibly nonzero differential is $d_3$. Let $u$ be the degree-three base generator. It cannot survive, because the sequence converges to $H^*(S^4;\mathbb Q)$ and that ring has zero degree-three part. It has no outgoing differential and its only possible incoming differential is from $E_3^{0,2}$. Hence there is $a\in H^2(F;\mathbb Q)$ with

$$
d_3a=u.
$$

The class $a$ is nonzero and, by the degree bound above, has a first vanishing power $a^r=0$ for some $r\geq2$. Multiplicativity says that $d_3$ is a graded derivation. Since $|a|=2$ is even,

$$
0=d_3(a^r)=r\,u\,a^{r-1}.
$$

But $E_3^{3,2r-2}=H^3(S^3;\mathbb Q)\otimes H^{2r-2}(F;\mathbb Q)$, in which $u a^{r-1}\ne0$ by minimality of $r$; also $r$ is nonzero over $\mathbb Q$. This is a contradiction. Thus no such [fiber bundle](../../../../../../fiber-bundle-split.md) exists. This is the special case of [a sphere cannot fibre over a lower-dimensional odd sphere](../../../../../../a-sphere-cannot-fibre-over-a-lower-dimensional-odd-sphere.md) required here.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [5](../../5.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
