<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Give the dual $M^*=\operatorname{Hom}_k(M,k)$ the contragredient action $(g\lambda)(m)=\lambda(g^{-1}m)$. If $\delta_h$ is the functional dual to the basis element $h\in G$, then

$$
g\delta_h=\delta_{gh}.
$$

Thus the map $h\mapsto\delta_h$ extends to a $kG$-isomorphism

$$
\boxed{kG\cong(kG)^*.}
$$

This is also the left-module form of the fact that a [group algebra is a symmetric algebra](../../../../../../group-algebra-is-a-symmetric-algebra.md).

If $P$ is finitely generated and projective, it is a direct summand of $(kG)^r$. Dualizing makes $P^*$ a direct summand of $((kG)^*)^r\cong(kG)^r$, so $P^*$ is projective. The converse follows by dualizing again and using $P\cong P^{**}$.

For any finite-dimensional algebra $A$, the module $A^*$ is injective because

$$
\operatorname{Hom}_A(-,A^*)\cong\operatorname{Hom}_k(-,k)
$$

is exact. Since $kG\cong(kG)^*$, free $kG$-modules are injective, and so are their projective direct summands. Conversely, duality sends injectives to projectives, so every finite-dimensional injective is projective. Hence [projective modules over a finite group algebra are injective](../../../../../../projective-modules-over-a-finite-group-algebra-are-injective.md).

Finally, let $P$ be indecomposable projective. It is also an indecomposable injective. Its nonzero [socle](../../../../../../socle-mathematics.md) contains a simple module $S$, and the [injective hull](../../../../../../injective-hull.md) $E(S)$ is a direct summand of $P$. Indecomposability forces $P=E(S)$. Since $S$ is essential in its injective hull, every simple submodule of $P$ equals $S$. Therefore

$$
\boxed{\operatorname{Soc}(P)\text{ is simple}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 138](../../../paper-138-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
