<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

The map

$$
\ell_v:V\to\mathbb R,
\qquad
\ell_v(x)=\langle v,x\rangle
$$

is a nonzero [linear functional](../../../../../linear-functional.md): otherwise $v$ would lie in the [radical of a bilinear form](../../../../../radical-of-a-bilinear-form.md), contradicting nondegeneracy. Its kernel is $v^\perp$, so the [rank-nullity theorem](../../../../../rank-nullity-theorem.md) gives $\dim v^\perp=n-1$. Antisymmetry gives $\langle v,v\rangle=-\langle v,v\rangle=0$, hence $v\in v^\perp$.

Suppose $w\in W$ is orthogonal to every vector of $W$. Since $W\subseteq v^\perp$, it is also orthogonal to $v$, and therefore to

$$
W\oplus\mathbb Rv=v^\perp.
$$

For a [nondegenerate bilinear form](../../../../../nondegenerate-bilinear-form.md), $(v^\perp)^\perp=\mathbb Rv$: both sides have dimension one and the latter is contained in the former. Thus $w\in W\cap\mathbb Rv=\{0\}$, proving that the restriction to $W$ is nondegenerate.

The space $W$ has dimension $n-2$ and again carries a nondegenerate antisymmetric form. Induction, starting from the zero-dimensional space, shows that $\dim W$ is even. Therefore $n=\dim W+2$ is even. Equivalently, every finite-dimensional [symplectic vector space](../../../../../symplectic-vector-space.md) has even dimension.

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
