<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a small category $C$, write $\widehat C=[C^{\mathrm{op}},\mathbf{Set}]$. Its objects are [categorical presheaves](../../../../../presheaf-category-theory.md) and its arrows [natural transformations](../../../../../natural-transformation.md). The terminal presheaf is the constant singleton, and products and [equalizers](../../../../../equaliser.md) are computed objectwise. Their restriction maps are induced by the corresponding set operations, so the objectwise universal properties are natural and give [finite limits](../../../../../finite-limit.md) in $\widehat C$.

For presheaves $F,G$, define the [exponential object](../../../../../exponential-object.md) by

$$
(G^F)(A)=\operatorname{Nat}(yA\times F,G),\qquad yA=C(-,A).
$$

For $u:B\to A$, restriction precomposes with $yu\times1_F$. Evaluation sends $(\alpha,x)$ at $A$ to $\alpha_A(1_A,x)$. Given $h:H\times F\to G$, its transpose sends $z\in H(A)$ to the transformation whose component at $B$ is

$$
(v:B\to A,x\in F(B))\longmapsto h_B(H(v)z,x).
$$

Naturality of $h$ proves this is a [natural transformation](../../../../../natural-transformation.md) and that the assignment is natural in $A$. Conversely evaluation reconstructs $h$. These constructions are inverse, proving the exponential universal property explicitly.

For the [subobject classifier](../../../../../subobject-classifier.md), let $\Omega(A)$ be the set of [sieves on a category](../../../../../sieve-category-theory.md) on $A$ and let $\Omega(u)$ take inverse image of [sieves on a category](../../../../../sieve-category-theory.md). The truth map $1\to\Omega$ selects the maximal [sieve on a category](../../../../../sieve-category-theory.md) at every stage. A [monomorphism](../../../../../monomorphism.md) of presheaves is objectwise injective, so identify it with $U\subseteq F$. Define

$$
\chi_U(x)=\{v:B\to A:F(v)x\in U(B)\},\qquad x\in F(A).
$$

This is a [sieve on a category](../../../../../sieve-category-theory.md), and restriction gives precisely inverse image, so $\chi_U$ is natural. Its value is maximal exactly when $x\in U(A)$, by testing the identity arrow. Thus $U$ is its pullback of truth. Uniqueness follows since membership of $v$ is detected by whether the restriction to $v$ is true. Smallness of $C$ makes all the displayed components and natural-transformation sets genuine sets. Hence **$\widehat C$ is an elementary topos**.

The same constructions work componentwise under the weaker slice hypothesis. Indeed,

$$
\operatorname{Nat}(yA\times F,G)\cong\operatorname{Nat}(F\circ\mathrm{dom},G\circ\mathrm{dom})_{C/A}.
$$

A component on $v:B\to A$ is simply a map $F(B)\to G(B)$, with the naturality conditions for triangles in $C/A$. Restricting to a small skeleton of an essentially small slice therefore makes this a set; the result determines the maps on all isomorphic slice objects. Likewise a [sieve on a category](../../../../../sieve-category-theory.md) on $A$ is a full downward-closed collection of objects of $C/A$, determined by its intersection with that small skeleton, so the collection of [sieves on a category](../../../../../sieve-category-theory.md) is a set. The restriction, evaluation and classifier proofs above are unchanged. This establishes the [slice-small presheaf construction](../../../../../slice-small-presheaf-construction.md).

For an example, take a discrete category with one object for every ordinal and no arrows other than identities. Each slice is the terminal category, but there is a proper class of pairwise nonisomorphic objects, so it is not equivalent to a small category.

**The large-category assertion needs a universe convention.** The constructions give all elementary-topos axioms in a larger universe in which those diagrams and their transformations are admitted. They do not imply local smallness in the original universe: for the discrete example, transformations from the constant singleton to the constant two-element presheaf are arbitrary ordinal-indexed binary families and do not form a set there. If “topos” is required to be locally small relative to that original universe, the unrestricted large-category assertion is false. With the usual larger-universe interpretation, the explicit component constructions prove the intended result; no assumption that the original category itself is essentially small is needed.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
