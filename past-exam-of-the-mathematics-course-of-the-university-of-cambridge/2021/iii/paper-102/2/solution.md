<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A Lie algebra is [semisimple](../../../../../semisimple-lie-algebra-split.md) when its soluble radical is zero. Its [Killing form](../../../../../killing-form.md) is

$$
B_L(x,y)=\operatorname{tr}(\operatorname{ad}x\,\operatorname{ad}y).
$$

The radical of this invariant symmetric form is an ideal. The solvability result behind the [Cartan criterion for semisimplicity](../../../../../cartan-criterion-for-semisimplicity.md) applied to that ideal shows that it is soluble; semisimplicity therefore makes it zero. Hence $B_L$ is nondegenerate.

An abelian subalgebra $H$ is a [Cartan subalgebra](../../../../../cartan-subalgebra.md) when its elements are semisimple and it is maximal toral, equivalently when $C_L(H)=H$. An arbitrary abelian subalgebra need not lie in one: in $\mathfrak{sl}_2$, the line spanned by the nilpotent matrix $e$ is abelian, whereas every element of a Cartan subalgebra is semisimple.

Let $H=C_L(h_0)$ for a regular $h_0\in H$, as allowed. Generalized eigenspaces of $\operatorname{ad}h_0$ give

$$
L=H\oplus[h_0,L].
$$

If $x\in H$ is orthogonal to $H$, invariance gives

$$
B_L(x,[h_0,y])=B_L([x,h_0],y)=0.
$$

Thus $x$ is orthogonal to all of $L$, and nondegeneracy gives $x=0$. Therefore $B_L|_H$ is nondegenerate.

The commuting semisimple maps $\{\operatorname{ad}h:h\in H\}$ can be simultaneously diagonalized. Consequently

$$
\boxed{L=H\oplus\bigoplus_{\alpha\in\Phi}L_\alpha,\qquad
L_\alpha=\{x:[h,x]=\alpha(h)x\ \forall h\in H\}.}
$$

Here $L_0=C_L(H)=H$, the nonzero weights $\Phi\subseteq H^*$ are the roots, and the Jacobi identity gives $[L_\alpha,L_\beta]\subseteq L_{\alpha+\beta}$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 102](../../paper-102-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
