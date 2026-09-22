<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the defining criterion that a [flat module](../../../../../../flat-module.md) $E$ makes $u\otimes1_E$ [injective](../../../../../../injective-function.md) for every [injective](../../../../../../injective-function.md) [module homomorphism](../../../../../../module-homomorphism.md) $u$. By [right exactness of the tensor product](../../../../../../right-exactness-of-the-tensor-product.md), preserving injections is equivalent to preserving every [short exact sequence](../../../../../../short-exact-sequence.md).

First assume $E$ is [flat](../../../../../../flat-module.md) over $A$, and fix a [maximal ideal](../../../../../../maximal-ideal.md) $\mathfrak m$. Let $u:U\hookrightarrow V$ be an [injection](../../../../../../injective-function.md) of $A_{\mathfrak m}$-modules. Regard it as an [injection](../../../../../../injective-function.md) of $A$-modules. There are natural [module isomorphisms](../../../../../../module-isomorphism.md)

$$
U\otimes_{A_{\mathfrak m}}E_{\mathfrak m}\cong U\otimes_AE,\qquad V\otimes_{A_{\mathfrak m}}E_{\mathfrak m}\cong V\otimes_AE.
$$

For example, $u_0\otimes(e/s)$ maps to $s^{-1}u_0\otimes e$, with inverse $u_0\otimes e\mapsto u_0\otimes(e/1)$. These are well-defined because every $s\notin\mathfrak m$ already acts invertibly on $U$. Under these [isomorphisms](../../../../../../isomorphism.md) the tensor map is $u\otimes_A1_E$, which is [injective](../../../../../../injective-function.md) by flatness. Thus $E_{\mathfrak m}$ is [flat](../../../../../../flat-module.md) over $A_{\mathfrak m}$.

For the converse, assume every $E_{\mathfrak m}$ is [flat](../../../../../../flat-module.md) over $A_{\mathfrak m}$ and take any [injection](../../../../../../injective-function.md) $u:U\hookrightarrow V$ of $A$-modules. By part (c), each $u_{\mathfrak m}$ is [injective](../../../../../../injective-function.md). Since [localization commutes with tensor products](../../../../../../localization-commutes-with-tensor-products.md), the [localization](../../../../../../localization-of-a-ring.md) of $u\otimes_A1_E$ identifies with

$$
u_{\mathfrak m}\otimes_{A_{\mathfrak m}}1_{E_{\mathfrak m}}:U_{\mathfrak m}\otimes_{A_{\mathfrak m}}E_{\mathfrak m}\longrightarrow V_{\mathfrak m}\otimes_{A_{\mathfrak m}}E_{\mathfrak m}.
$$

It is [injective](../../../../../../injective-function.md) by the assumed local flatness. Apply part (c) again, now to $u\otimes_A1_E$, to conclude that it is [injective](../../../../../../injective-function.md) globally. Since $u$ was arbitrary, $E$ is [flat](../../../../../../flat-module.md). Therefore

$$
\boxed{E\text{ is <flat> over }A\iff E_{\mathfrak m}\text{ is <flat> over }A_{\mathfrak m}\text{ for every maximal }\mathfrak m.}
$$

This proves [flatness is local](../../../../../../flatness-is-local.md) without any finite-generation hypothesis.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
