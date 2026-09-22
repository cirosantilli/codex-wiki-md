<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the stable finite-dimensional description. Define addition by block sum, $[u]+[v]=[\operatorname{diag}(u,v)]$. Stabilizations and [homotopies](../../../../../../homotopy.md) preserve block sums, so this is well-defined. Associativity is immediate after identifying the three blocks; the identity class is zero.

Swapping two blocks is conjugation by a permutation unitary. Every finite-dimensional unitary is joined to the identity, since the matrix spectral theorem writes it as $e^{iA}$ with $A$ self-adjoint. Conjugation along that path gives a [homotopy](../../../../../../homotopy.md) swapping the blocks, proving commutativity.

The inverse of $[u]$ is $[u^{-1}]$. To verify it rather than assuming a group structure, first stabilize to equal-sized blocks and put

$$
R_t=\begin{pmatrix}\cos t\,I&-\sin t\,I\\\sin t\,I&\cos t\,I\end{pmatrix}.
$$

The invertible [homotopy](../../../../../../homotopy.md)

$$
\operatorname{diag}(u,I)\,R_t\operatorname{diag}(I,u^{-1})R_t^{-1},\qquad0\leq t\leq\pi/2,
$$

starts at $\operatorname{diag}(u,u^{-1})$ and ends at the identity. Thus **$\boxed{K^1(X)\text{ is an abelian group}.}$** The constructions are continuous in $x$ and remain valid for maps into $GL_N$; using polar factors also makes them [homotopies](../../../../../../homotopy.md) in the unitary model.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [7](../../7.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
