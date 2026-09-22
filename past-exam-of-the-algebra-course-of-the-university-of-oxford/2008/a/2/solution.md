<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [composition series](../../../../composition-series.md) is a chain $0=V_0\subsetneq V_1\subsetneq\cdots\subsetneq V_r=V$ of submodules with every factor $V_i/V_{i-1}$ simple; its length is $r$. Suppose $0\subset S\subset V$ is one of length two, and put $T=V/S$.

For any nonzero proper [submodule](../../../../submodule.md) $U$, either $U\cap S=S$ or $U\cap S=0$, by simplicity of $S$. In the first case, simplicity of $V/S$ forces $U=S$. In the second, the quotient map embeds $U$ nontrivially into $T$, so $U\cong T$ and its [image](../../../../image-of-a-function.md) is all of $T$. Hence $V=S\oplus U$, and $V/U\cong S$. Thus every nonzero proper [submodule](../../../../submodule.md) is simple and has simple quotient; every [composition series](../../../../composition-series.md) has length two.

The [Jordan–Hölder theorem](../../../../jordan-holder-theorem.md) states that any two [composition series](../../../../composition-series.md) of a finite-length module have equal length and the same multiset of simple factors, up to isomorphism and order. The preceding argument proves this for length two: either $U=S$, giving factors $S,T$, or $U\ne S$, giving factors $T,S$.

The map $A\to S$, $a\mapsto ax$, is a surjective [module homomorphism](../../../../module-homomorphism.md) with [kernel](../../../../kernel-of-a-linear-map-split.md) $I=\operatorname{Ann}_A(x)$. The [first isomorphism theorem for modules](../../../../first-isomorphism-theorem-for-modules.md) gives $A/I\cong S$ as left modules; $I$ need only be a [left ideal](../../../../left-ideal.md). Every [simple module](../../../../irreducible-module.md) is cyclic, since any nonzero $x$ generates a nonzero [submodule](../../../../submodule.md). As a quotient of the finite-dimensional regular module $A$, it is finite-dimensional. Extend $I$ to a [composition series](../../../../composition-series.md) of $A$; its simple quotient $A/I$ is one of the factors. Jordan-Hölder shows that its isomorphism type belongs to the fixed finite list of factors of any one [composition series](../../../../composition-series.md) of $A$. Hence **there are finitely many simple-module isomorphism types**.

For the final assertion let $W$ be the [image](../../../../image-of-a-function.md) of $\psi$. Its [kernel](../../../../kernel-of-a-linear-map-split.md) is $\bigcap I_j$. We prove $W=\prod S_j$ by induction on $k$. It is true for $k=1$. Projection onto the first $k-1$ factors is onto by induction. Its [kernel](../../../../kernel-of-a-linear-map-split.md) on $W$ is a [submodule](../../../../submodule.md) of $S_k$, so is zero or $S_k$. If zero, $W\cong\prod_{j<k}S_j$. But its projection onto $S_k$ is onto, making $S_k$ a [composition factor](../../../../composition-factor.md) of that product, contrary to Jordan-Hölder and the pairwise distinct types. Thus the [kernel](../../../../kernel-of-a-linear-map-split.md) is all of $S_k$. Surjectivity on the first factors together with this [kernel](../../../../kernel-of-a-linear-map-split.md) proves $W$ is the entire product. The first isomorphism theorem now gives

$$
\boxed{A/\bigcap_{j=1}^kI_j\cong S_1\times\cdots\times S_k}
$$

as left $A$-modules, without asserting that the left ideals are two-sided.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the algebra course of the University of Oxford](../../../split.md)
5. [Algebra course of the University of Oxford](../../../../algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
