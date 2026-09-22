<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

By [irreducible traceless matrix Lie algebra is semisimple](../../../../irreducible-traceless-matrix-lie-algebra-is-semisimple.md), let $R$ be the [solvable radical](../../../../radical-of-a-lie-algebra.md). [Lie's theorem](../../../../lie-s-theorem.md) triangularizes its action, with finitely many diagonal [characters](../../../../character-of-a-representation.md) $\lambda_i:R\to\mathbb C$, and supplies a nonzero common [eigenspace](../../../../eigenspace.md) for one of them. For $x\in L$, conjugation by $e^{tx}$ preserves $R$ and gives an equivalent [representation](../../../../group-representation.md) of it. Thus the multiset of [characters](../../../../character-of-a-representation.md) $\lambda_i\circ e^{t\operatorname{ad}x}$ is constant. Each [character](../../../../character-of-a-representation.md) varies continuously in $t$ and has values in that finite set of [characters](../../../../character-of-a-representation.md), so it is individually constant. Differentiating at zero gives $\lambda_i([x,r])=0$ for all $r\in R$.

Choose a common [eigenspace](../../../../eigenspace.md) $V_\lambda\ne0$. For $v\in V_\lambda$,

$$
r(xv)=x(rv)+[r,x]v=\lambda(r)xv+\lambda([r,x])v=\lambda(r)xv.
$$

Thus $V_\lambda$ is $L$-invariant, so irreducibility makes it all of $\mathbb C^n$. Every element of $R$ acts as a scalar. Its [trace](../../../../matrix-trace.md) is zero because $L\subseteq\mathfrak{sl}_n$, so that scalar is zero. Faithfulness of the [matrix](../../../../matrix.md) inclusion gives $R=0$. Hence $\boxed{L\text{ is semisimple}}$.

One sufficient diagonal-[matrix](../../../../matrix.md) condition for simplicity is that $L$ contain **all traceless [diagonal matrices](../../../../diagonal-matrix.md)**. Indeed invariance under their adjoint actions then decomposes $L$ into that diagonal algebra and some [matrix](../../../../matrix.md)-unit spaces $\mathbb Ce_{ij}$. Put a directed edge $j\to i$ when $e_{ij}\in L$. Irreducibility makes the directed graph strongly connected; otherwise a terminal component spans a proper invariant coordinate subspace. Bracketing [matrix units](../../../../matrix-unit.md) along a simple directed path supplies the [matrix unit](../../../../matrix-unit.md) between its endpoints. Strong connectivity therefore supplies every off-[diagonal matrix](../../../../diagonal-matrix.md) unit, so $L=\mathfrak{sl}_n$, which is simple. The mere existence of a [diagonal matrix](../../../../diagonal-matrix.md) with distinct diagonal entries would not be a sufficient condition.

For the specified construction, $H$ has [dimension](../../../../dimension-vector-space.md) two. Its diagonal adjoint action and the twelve distinct nonzero [weights](../../../../weight-of-a-representation.md) give a [direct sum](../../../../direct-sum.md) $L=H\oplus\bigoplus_{i=1}^{12}\mathbb Cg_i$, of [dimension](../../../../dimension-vector-space.md) fourteen. The stated bracket condition and the [weight](../../../../weight-of-a-representation.md)-vector relations make it a [Lie algebra](../../../../lie-algebra-split.md). A subspace invariant under it is invariant under all the $g_i$ and hence their associative algebra, so it acts irreducibly on $\mathbb C^7$. The preceding result makes it semisimple.

Use [prime-dimensional faithful irreducible module forces simplicity](../../../../prime-dimensional-faithful-irreducible-module-forces-simplicity.md). To see this, decompose the algebra into simple [ideals](../../../../ideal-of-a-lie-algebra.md). Complete reducibility for one [ideal](../../../../ideal-of-a-lie-algebra.md) and commutation with the others make its isotypic component invariant under the whole algebra, hence all of the [representation](../../../../group-representation.md). Writing that component as $W\otimes\operatorname{Hom}(W,V)$ and repeating produces a [tensor product](../../../../tensor-product.md) of irreducibles for the simple [ideals](../../../../ideal-of-a-lie-algebra.md). Faithfulness makes every factor nontrivial, of [dimension](../../../../dimension-vector-space.md) at least two. Their dimensions multiply to seven, so only one factor is possible. Thus the constructed $L$ is simple.

The diagonal algebra $H$ is toral, and its centralizer inside $L$ is just $H$, since no $g_i$ has zero [weight](../../../../weight-of-a-representation.md). A maximal [toral subalgebra](../../../../toral-subalgebra.md) containing $H$ lies in that centralizer, so equals $H$; it is a [Cartan subalgebra](../../../../cartan-subalgebra.md). Thus the rank is two and the twelve [weights](../../../../weight-of-a-representation.md) are the [roots](../../../../root-of-a-root-system.md). Pair them as $\alpha_{i+6}=-\alpha_i$. The opposite-[root](../../../../root-of-a-root-system.md) brackets have [weight](../../../../weight-of-a-representation.md) zero and belong to $H$. For distinct $i,j\le6$, the sum cannot be zero, and the supplied [root](../../../../root-of-a-root-system.md)-bracket result says their bracket is nonzero exactly when $\alpha_i+\alpha_j$ is a [root](../../../../root-of-a-root-system.md). This is equivalent to $-\alpha_i-\alpha_j$ being a [root](../../../../root-of-a-root-system.md), proving the requested equivalence for the paired brackets.

Among rank-two [simple root](../../../../simple-root.md) systems, $A_2,B_2,G_2$ have respectively six, eight and twelve [roots](../../../../root-of-a-root-system.md). Therefore

$$
\boxed{L\text{ has type }G_2.}
$$

Choose [simple roots](../../../../simple-root.md) $\alpha$ short and $\beta$ long. In $G_2$, $\beta+\alpha$ and $\beta+2\alpha$ are [roots](../../../../root-of-a-root-system.md). Renumber with $g_1\in L_\alpha$, $g_3\in L_\beta$, $g_4\in L_{\beta+\alpha}$ and $g_5\in L_{\beta+2\alpha}$, retaining opposite partners in the other six positions. [Root spaces](../../../../root-space.md) are one dimensional, and the allowed bracket equality gives

$$
\boxed{[g_3,g_1]=\mu_1g_4,\qquad[g_4,g_1]=\mu_2g_5,\qquad\mu_1\mu_2\ne0.}
$$

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../split.md)
5. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
