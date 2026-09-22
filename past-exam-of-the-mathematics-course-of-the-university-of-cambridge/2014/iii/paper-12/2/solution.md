<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Define [compactly supported cohomology](../../../../../compactly-supported-cohomology.md) by

$$
\boxed{H_{ct}^q(X;A)=\varinjlim_{K\subseteq X\text{ compact}}H^q(X,X\setminus K;A).}
$$

For $K\subseteq L$, the transition map is induced by the identity map of pairs $(X,X\setminus L)\to(X,X\setminus K)$. Equivalently, take the [cochain complex](../../../../../cochain-complex.md) of [singular cochains](../../../../../singular-cochain.md) that vanish on every chain contained in the complement of some compact set. Directed unions are exact, giving the same definition.

For $\mathbb R$, the intervals $[-a,a]$, $a>0$, are cofinal among compact subsets. The complement has two contractible components. The [long exact sequence](../../../../../long-exact-sequence.md) in [relative cohomology](../../../../../relative-cohomology.md) contains the diagonal map $\mathbb Z\to\mathbb Z\oplus\mathbb Z$, so its cokernel is $H^1(\mathbb R,\mathbb R\setminus[-a,a])\cong\mathbb Z$, and all the other relative groups vanish. Enlarging the interval preserves the generator given by the difference of the two ends. Therefore

$$
\boxed{H_{ct}^q(\mathbb R;\mathbb Z)=\begin{cases}\mathbb Z,&q=1,\\0,&q\ne1.\end{cases}}
$$

For the [compact-support comparison with a one-point compactification](../../../../../compact-support-comparison-with-a-one-point-compactification.md), write $Y=X^+$. The assumed Hausdorff [one-point compactification](../../../../../alexandroff-extension.md) is compact; a compact subset $K\subseteq X$ is closed in $Y$. The [Excision theorem](../../../../../excision-theorem.md) removes $\{\infty\}$ from the pair $(Y,Y\setminus K)$, because its closure lies inside the open second member. Thus

$$
H^q(X,X\setminus K)\cong H^q(Y,Y\setminus K).
$$

Complements of compact subsets of $X$ are exactly the open neighbourhoods of $\infty$ in $Y$. The hypothesis supplies a cofinal family of contractible such neighbourhoods $U$. For every one, the [long exact sequence](../../../../../long-exact-sequence.md) of the pair identifies

$$
H^q(Y,U)\cong\widetilde H^q(Y).
$$

In degree zero, this is the kernel of evaluation on the component of $\infty$, identified with [reduced cohomology](../../../../../reduced-cohomology.md) by subtracting the constant value there. In degree one the map $H^0(Y)\to H^0(U)\cong\mathbb Z$ is surjective; in higher degrees the positive cohomology of $U$ vanishes. These identifications are natural for inclusions of contractible neighbourhoods. Passing to the [direct limit](../../../../../direct-limit-of-abelian-groups.md) proves

$$
\boxed{H_{ct}^*(X)\cong\widetilde H^*(X^+).}
$$

For the specified disjoint union of lines, a compact subset meets only finitely many components and is bounded in each. Finite unions $F\times[-a,a]$, with $F\subset\mathbb Z$ finite, are cofinal. Applying the preceding relative calculation componentwise gives

$$
\boxed{H_{ct}^q(\mathbb Z\times\mathbb R;\mathbb Z)=\begin{cases}\displaystyle\bigoplus_{j\in\mathbb Z}\mathbb Z,&q=1,\\0,&q\ne1.\end{cases}}
$$

The [one-point compactification](../../../../../alexandroff-extension.md) $W$ of this space is the [Hawaiian earring](../../../../../hawaiian-earring.md): each line becomes a circle by adding the common point $\infty$, and every neighbourhood of $\infty$ contains all but finitely many whole circles. On the remaining finitely many circles it contains neighbourhoods of the common point. This describes exactly the shrinking-circle topology. In particular $W$ is not locally contractible at $\infty$: every such neighbourhood contains a whole circle, whose generator remains nontrivial under the retraction $W\to S^1$ that collapses all the other circles.

For integral [singular cohomology](../../../../../singular-cohomology.md), the comparison **does not hold**. Here is a degree-two obstruction that takes account of the shrinking-circle topology. The standard [rational summand in Hawaiian earring homology](../../../../../rational-summand-in-hawaiian-earring-homology.md) theorem gives a [direct summand](../../../../../direct-summand.md) $\mathbb Q$ in $H_1(W;\mathbb Z)$. The [universal coefficient theorem for cohomology](../../../../../universal-coefficient-theorem-for-cohomology.md) injects

$$
\operatorname{Ext}_{\mathbb Z}^1(H_1(W;\mathbb Z),\mathbb Z)\hookrightarrow H^2(W;\mathbb Z).
$$

The summand $\mathbb Q$ therefore contributes the [nonzero Ext of the rationals with integer coefficients](../../../../../nonzero-ext-of-the-rationals-with-integer-coefficients.md).

For completeness, this last algebraic assertion has an explicit proof. Present $\mathbb Q$ using generators $a_n=1/n!$ and relations $a_n-(n+1)a_{n+1}=0$, $n\geq1$. The corresponding free resolution shows that $\operatorname{Ext}^1_{\mathbb Z}(\mathbb Q,\mathbb Z)$ is the cokernel of

$$
\prod_{n\geq1}\mathbb Z\longrightarrow\prod_{n\geq1}\mathbb Z,\qquad (u_n)\longmapsto(u_n-(n+1)u_{n+1}).
$$

The constant sequence $(1,1,\ldots)$ is not in the image. Otherwise iteration would give

$$
u_1=\sum_{j=1}^N j!+(N+1)!u_{N+1}\quad\text{for every }N.
$$

For large $N$, the factorial sum exceeds $|u_1|$ but is less than $(N+1)!-|u_1|$, making that congruence impossible. Thus the cokernel is nonzero. It follows that

$$
\boxed{H_{ct}^2(\mathbb Z\times\mathbb R;\mathbb Z)=0,\qquad\widetilde H^2(W;\mathbb Z)\ne0,}
$$

which proves the failure of the claimed isomorphism. The ingredient concerning the [Hawaiian earring](../../../../../hawaiian-earring.md) is its singular-homology structure theorem, not the homology of an infinite [CW complex](../../../../../cw-complex.md) wedge of circles; these topologies differ.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
