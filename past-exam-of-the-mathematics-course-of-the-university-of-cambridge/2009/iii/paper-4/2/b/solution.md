<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $V$ be an irreducible $G$-module with character $\chi\in\operatorname{Irr}(G\mid\theta)$, and let $W=V_\theta\ne0$ be its $\theta$-[isotypic component](../../../../../../isotypic-component.md). It is invariant under the [inertia group of a character](../../../../../../inertia-group-of-a-character.md) $T$. The sum of its $G$-translates is a nonzero $G$-submodule, so irreducibility makes it all of $V$. Translates associated with different cosets $gT$ have distinct $N$-types and hence form a [direct sum](../../../../../../direct-sum.md):

$$
V=\bigoplus_{g\in\mathcal R}gW.
$$

To see that $W$ is irreducible over $T$, let $0\ne W_0\subseteq W$ be a $T$-submodule. Then $\sum_{g\in\mathcal R}gW_0$ is a nonzero $G$-submodule of $V$, hence equals $V$. Its $\theta$-isotypic part is exactly $W_0$, whereas the corresponding part of $V$ is $W$. Thus $W_0=W$.

Let $\xi$ be the [irreducible character](../../../../../../irreducible-character.md) of $W$ as a $T$-module. It lies over $\theta$, and the natural map of [induced representations](../../../../../../induced-representation.md)

$$
\mathbb C[G]\otimes_{\mathbb C[T]}W\longrightarrow V,\qquad g\otimes w\longmapsto gw
$$

is an isomorphism: it identifies each summand with the corresponding $gW$, and these summands are direct and exhaust $V$. Consequently $\chi=\xi^G$, proving surjectivity of induction on the stated sets.

For injectivity, the construction in (a) shows that the $\theta$-isotypic component of $\operatorname{Ind}_T^G W$ is exactly $1\otimes W$, with its original $T$-action. Isomorphic induced $G$-modules therefore have isomorphic intrinsic $\theta$-components as $T$-modules. Since complex representations with the same character are isomorphic, $\xi_1^G=\xi_2^G$ forces $\xi_1=\xi_2$. Hence the [Clifford correspondence](../../../../../../clifford-correspondence.md) is the bijection

$$
\boxed{\operatorname{Irr}(T\mid\theta)\xrightarrow{\ \xi\mapsto\xi^G\ }\operatorname{Irr}(G\mid\theta),}
$$

whose inverse takes the character of the $\theta$-isotypic component.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
