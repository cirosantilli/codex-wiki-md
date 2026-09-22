<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

We prove [power set in a generic extension](../../../../../../power-set-in-a-generic-extension.md) by bounding possible subnames in the ground model, rather than presupposing the desired [power set](../../../../../../power-set.md) in $M[G]$. Let $x=\tau^G$, and let $S=\{\rho:\exists r\,((\rho,r)\in\tau)\}$. In $M$ form

$$
U=\{(\rho,p)\in S\times\mathbb P:\exists r\,((\rho,r)\in\tau\land p\leq r)\},\qquad B=\mathcal P^M(U).
$$

Every $\nu\in B$ is a [forcing name](../../../../../../forcing-name.md). Its value is a [subset](../../../../../../subset.md) of $x$: an active pair $(\rho,p)\in\nu$ has $p\leq r$ for some $(\rho,r)\in\tau$, so $p\in G$ implies $r\in G$ and $\rho^G\in x$.

Now take any $y\in M[G]$ with $y\subseteq x$, and choose a [forcing name](../../../../../../forcing-name.md) $\sigma\in M$ with $\sigma^G=y$. By [axiom schema of separation](../../../../../../axiom-schema-of-specification.md) and definability of the [syntactic forcing relation](../../../../../../syntactic-forcing-relation.md),

$$
\nu_\sigma=\{(\rho,p)\in U:p\Vdash^*\rho\in\sigma\}\in B.
$$

The [atomic membership truth lemma for forcing](../../../../../../atomic-membership-truth-lemma-for-forcing.md) shows $\nu_\sigma^G=y$. One inclusion follows immediately from its soundness direction. For the other, if $a\in y\subseteq x$, choose $(\rho,r)\in\tau$ with $r\in G$ and $\rho^G=a$. The truth direction supplies $p\in G$ forcing $\rho\in\sigma$; strengthen within $G$ below $p$ and $r$ to obtain an active pair in $\nu_\sigma$ representing $a$.

Finally the ground-model [forcing name](../../../../../../forcing-name.md)

$$
\Pi_\tau=\{(\nu,p):\nu\in B,\ p\in\mathbb P\}
$$

exists by [Axiom schema of replacement](../../../../../../axiom-schema-of-replacement.md) and the ground-model [power set](../../../../../../power-set.md) axiom. Since $G$ is nonempty, all $\nu\in B$ contribute their values, and

$$
\boxed{\Pi_\tau^G=\{y\in M[G]:y\subseteq\tau^G\}=\mathcal P^{M[G]}(x).}
$$

This [set](../../../../../../set-split.md) belongs to $M[G]$ by the definition of a [generic extension](../../../../../../generic-extension.md). The construction uses all conditions in the outer pairs and therefore does not require a greatest condition in $\mathbb P$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
