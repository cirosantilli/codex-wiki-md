<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [elementary topos](../../../../../elementary-topos.md) definition: a [category](../../../../../category-split.md) with [finite limits](../../../../../finite-limit.md), [exponential objects](../../../../../exponential-object.md), and a [subobject classifier](../../../../../subobject-classifier.md). The indexing category $\mathbb C$ is assumed small, as usual, and $\widehat{\mathbb C}=[\mathbb C^{\mathrm{op}},\mathbf{Set}]$ denotes its [presheaf category](../../../../../presheaf-category.md). A [finite limit](../../../../../finite-limit.md) of [categorical presheaves](../../../../../presheaf-category-theory.md) is formed objectwise: at $c$ take the corresponding limit of sets, and apply the universal property to induce restriction maps. The terminal [categorical presheaf](../../../../../presheaf-category-theory.md) is the constant singleton, so this supplies all required [finite limits](../../../../../finite-limit.md).

For [categorical presheaves](../../../../../presheaf-category-theory.md) $A,B$, write $yc=\mathbb C(-,c)$ and define

$$
(B^A)(c)=\operatorname{Nat}(yc\times A,B).
$$

For $h:d\to c$, restriction is precomposition with $yh\times1_A$. Evaluation sends $(\theta,a)$ at $c$ to $\theta_c(1_c,a)$. Given $\phi:H\times A\to B$, its transpose sends $x\in H(c)$ to the [natural transformation](../../../../../natural-transformation.md) whose component at $d$ is

$$
(h:d\to c,a\in A(d))\longmapsto\phi_d(H(h)x,a).
$$

Naturality of $\phi$ proves this is a [natural transformation](../../../../../natural-transformation.md); naturality in $c$ proves it is a map $H\to B^A$. Conversely evaluation recovers $\phi$, and these constructions are inverse. Therefore

$$
\widehat{\mathbb C}(H\times A,B)\cong\widehat{\mathbb C}(H,B^A),
$$

so the [presheaf category](../../../../../presheaf-category.md) is [Cartesian closed](../../../../../cartesian-closed-category.md).

Define $\Omega(c)$ to be the set of [sieves on a category](../../../../../sieve-category-theory.md) with codomain $c$. For $h:d\to c$, let $\Omega(h)S=h^*S=\{k:e\to d:hk\in S\}$, and let $\top:1\to\Omega$ select the maximal sieve at each object. For a [subobject](../../../../../subobject.md) $U\hookrightarrow X$, define its characteristic map by

$$
\chi_c(x)=\{h:d\to c:X(h)x\in U(d)\}.
$$

The restriction closure of $U$ makes this a [sieve on a category](../../../../../sieve-category-theory.md), and the formula commutes with pullback of [sieves on a category](../../../../../sieve-category-theory.md), so $\chi$ is natural. It is maximal exactly when $1_c$ belongs to it, equivalently when $x\in U(c)$; hence the pullback of $\top$ along $\chi$ is $U$. Uniqueness is also explicit: naturality forces $h\in\chi_c(x)$ exactly when the restriction $X(h)x$ lies in the truth pullback at $d$. **Thus the sieve presheaf is a subobject classifier, and every small presheaf category is an elementary topos.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
