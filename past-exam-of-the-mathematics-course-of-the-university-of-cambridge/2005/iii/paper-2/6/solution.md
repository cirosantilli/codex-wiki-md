<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Work with a finite-dimensional complex [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md). The [Dynkin diagram](../../../../../dynkin-diagram.md) is obtained from its intrinsic [root system](../../../../../root-system.md), with several structure theorems entering the construction.

First choose a [Cartan subalgebra](../../../../../cartan-subalgebra.md) $\mathfrak h$. The semisimple structure theory gives the [root-space decomposition](../../../../../root-space-decomposition.md)

$$
\mathfrak g=\mathfrak h\oplus\bigoplus_{\alpha\in\Phi}\mathfrak g_\alpha,\qquad
\mathfrak g_\alpha=\{X:[H,X]=\alpha(H)X\text{ for all }H\in\mathfrak h\}.
$$

The nonzero [roots](../../../../../root-of-a-root-system.md) span $\mathfrak h^*$, [root spaces](../../../../../root-space.md) have [dimension](../../../../../dimension-vector-space.md) one, and every [root](../../../../../root-of-a-root-system.md) has its negative. The rank is $r=\dim\mathfrak h$.

Next use the [Killing form](../../../../../killing-form.md). Its nondegeneracy on $\mathfrak h$ and its positive-definite restriction to the real [coroot](../../../../../coroot.md) span identify the real [root](../../../../../root-of-a-root-system.md) span $E=\mathbb R\Phi$ with a Euclidean space. Explicitly, if $t_\lambda=\mathcal B^{-1}(\lambda)$, put $(\lambda,\mu)=B(t_\lambda,t_\mu)$. The [sl2 subalgebra associated with a root](../../../../../sl2-subalgebra-associated-with-a-root.md) supplies its normalized [coroot](../../../../../coroot.md) $H_\alpha$ and the integral pairing

$$
\beta(H_\alpha)=\frac{2(\beta,\alpha)}{(\alpha,\alpha)}\in\mathbb Z.
$$

The [root-string theorem](../../../../../root-string-theorem.md) makes the reflection $s_\alpha(\beta)=\beta-\beta(H_\alpha)\alpha$ permute $\Phi$. Together with the absence of multiples other than $\pm\alpha$, this shows that $\Phi$ is a finite [reduced root system](../../../../../reduced-root-system.md) and a [crystallographic root system](../../../../../crystallographic-root-system.md). These properties come from [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) theory, not from the diagram's definition.

Choose a vector in $E$ that is not perpendicular to any [root](../../../../../root-of-a-root-system.md). Define the [positive roots](../../../../../positive-root.md) by positive inner product with this vector. The [simple roots](../../../../../simple-root.md) are those [positive roots](../../../../../positive-root.md) that cannot be expressed as sums of two [positive roots](../../../../../positive-root.md). Root-system theory shows that they form a [basis](../../../../../basis.md) $\Delta=\{\alpha_1,\ldots,\alpha_r\}$, and each [root](../../../../../root-of-a-root-system.md) is an integer combination of them with coefficients all of one sign. Distinct [simple roots](../../../../../simple-root.md) have nonpositive inner product.

Use the standard [Cartan matrix](../../../../../cartan-matrix.md) convention

$$
A_{ij}=\alpha_i(H_{\alpha_j})=\frac{2(\alpha_i,\alpha_j)}{(\alpha_j,\alpha_j)}.
$$

There is one diagram vertex for each [simple root](../../../../../simple-root.md). For $i\ne j$, the integral off-diagonal entries are nonpositive and

$$
A_{ij}A_{ji}=4\cos^2\theta_{ij}\in\{0,1,2,3\}.
$$

Connect the two vertices with respectively zero, one, two or three edges. The corresponding angles are $90^\circ,120^\circ,135^\circ,150^\circ$. A multiple edge carries an arrow **toward the shorter [root](../../../../../root-of-a-root-system.md)**. For joined vertices, the length ratio is determined by $A_{ij}/A_{ji}=(\alpha_i,\alpha_i)/(\alpha_j,\alpha_j)$; hence the diagram records both angle and relative length.

For example, $\mathfrak{sl}_3$ has [simple roots](../../../../../simple-root.md) $L_1-L_2$ and $L_2-L_3$, giving two equal-length vertices joined by one edge: type $A_2$. For $\mathfrak{sp}_4$, take $\alpha_1=L_1-L_2$ and $\alpha_2=2L_2$. Then

$$
A=\begin{pmatrix}2&-1\\-2&2\end{pmatrix},
$$

so the two vertices have a double edge directed toward $\alpha_1$, the shorter [root](../../../../../root-of-a-root-system.md): type $C_2$.

Finally, orthogonal irreducible components of the [root system](../../../../../root-system.md) correspond to the simple [ideals of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md) in the [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md), so its diagram is the disjoint union of their connected diagrams. Conjugacy of [Cartan subalgebras](../../../../../cartan-subalgebra.md) and the [Weyl group](../../../../../weyl-group.md) action on choices of [positive roots](../../../../../positive-root.md) make the resulting diagram independent of these choices up to isomorphism. **Thus the vertices, edge multiplicities, arrows and connected components encode the simple-root geometry and the simple-ideal decomposition.**

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
