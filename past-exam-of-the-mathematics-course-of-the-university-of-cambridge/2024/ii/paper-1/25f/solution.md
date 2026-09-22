<h1 id="25f/solution">Solution</h1>

↑ **Parent:** [25F](../25f.md)

A nonempty topological space is irreducible when it is not the union of two proper closed subsets, equivalently when any two nonempty open subsets intersect.

The Zariski topology on $\mathbb A^n$ is Noetherian because $k[x_1,\ldots,x_n]$ satisfies the ascending chain condition on [ideals](../../../../../ideal.md). Suppose a closed set $X$ that is not a finite union of irreducible closed sets were minimal among such counterexamples. It is reducible, say $X=X_1\cup X_2$ with both $X_i$ proper closed subsets. Minimality expresses each $X_i$ as a finite union of irreducible closed sets, and combining those decompositions contradicts the choice of $X$. Thus every closed $X$ has a finite irreducible decomposition.

Using $x_3=x_2^2$, the second defining [polynomial](../../../../../polynomial-split.md) reduces to

$$
x_1^2-x_2^2-x_2^4+x_3^2=x_1^2-x_2^2.
$$

Consequently

$$
Z(x_3-x_2^2,x_1^2-x_2^2-x_2^4+x_3^2)
=
Z(x_3-x_2^2,x_1-x_2)
\cup
Z(x_3-x_2^2,x_1+x_2).
$$

Each component is the image of $t\mapsto(\pm t,t,t^2)$ and is isomorphic to $\mathbb A^1$, hence irreducible. In characteristic two the two displayed components coincide.

Suppose a [polynomial](../../../../../polynomial-split.md) $P(x,y)=\sum_{j=0}^m p_j(x)y^j$ vanishes on every $(x,e^x)$. Then

$$
\sum_{j=0}^m p_j(x)e^{jx}=0
$$

as an [entire function](../../../../../entire-function.md). These exponential-polynomial [functions](../../../../../function-split.md) are linearly independent: applying $(D-m)^{\deg p_m+1}$ kills the term with largest exponent, while it acts injectively on $p_j(x)e^{jx}$ for $j<m$; induction on the number of terms finishes the proof. Hence every $p_j$ is zero, so no nonzero [polynomial](../../../../../polynomial-split.md) vanishes on the graph. Its Zariski closure is all of $\mathbb A^2$.

Finally refine an open cover of an affine variety $X$ by distinguished opens $D(f_j)$, choosing one inside an original member around each point. Since these distinguished opens cover,

$$
V((f_j)_j)=\varnothing.
$$

The [Hilbert Nullstellensatz](../../../../../hilbert-nullstellensatz.md) implies that the $f_j$ generate the unit [ideal](../../../../../ideal.md). Thus

$$
1=g_1f_{j_1}+\cdots+g_rf_{j_r}
$$

for finitely many of them, so $D(f_{j_1}),\ldots,D(f_{j_r})$ cover $X$. The corresponding original [open sets](../../../../../open-set.md) form a finite subcover. This is [quasi-compactness of an affine variety](../../../../../quasi-compactness-of-an-affine-variety.md).

## ↑ Ancestors (10)

1. [25F](../25f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
