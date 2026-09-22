<h1 id="18h/solution">Solution</h1>

↑ **Parent:** [18H](../18h.md)

A [K-isomorphism](../../../../../k-isomorphism.md) $L\to L'$ is a [field isomorphism](../../../../../field-isomorphism.md) fixing every element of $K$. The [field automorphism group](../../../../../field-automorphism-group.md) $\operatorname{Aut}_K(L)$ consists of such isomorphisms $L\to L$, with composition.

If an isomorphism sends $\alpha$ to $\beta$, it takes every [polynomial](../../../../../polynomial-split.md) relation over $K$ for $\alpha$ to the same relation for $\beta$; the monic [minimal polynomials](../../../../../minimal-polynomial.md) coincide. Conversely, if their common [minimal polynomial](../../../../../minimal-polynomial.md) is $m$, evaluation induces [field isomorphisms](../../../../../field-isomorphism.md) $K[X]/(m)\cong K(\alpha)$ and $K[X]/(m)\cong K(\beta)$. Their composite sends $\alpha$ to $\beta$ and fixes $K$.

An [automorphism](../../../../../automorphism.md) of $K(\alpha)$ sends $\alpha$ to a root of $m$ inside $K(\alpha)$ and is determined by this image. More precisely the [field automorphism group](../../../../../field-automorphism-group.md) permutes the set of roots of $m$ lying in this field, a set of size $s\leq d$. This action is faithful because fixing $\alpha$ fixes the generated field. Thus $\operatorname{Aut}_K(K(\alpha))$ embeds in $S_s$, and then in $S_d$ by fixing $d-s$ extra labels. In particular it is finite. This argument also covers inseparable [minimal polynomials](../../../../../minimal-polynomial.md).

For an example not isomorphic even as abstract fields, take $K=\mathbb F_p(t)$, let $\alpha$ generate $\mathbb F_{p^p}$ over $\mathbb F_p$, and put $\beta=t^{1/p}$. The constant-field [minimal polynomial](../../../../../minimal-polynomial.md) of $\alpha$ remains irreducible over the [rational function](../../../../../rational-function.md) field: if it factored over $\mathbb F_p(t)$, each monic factor's coefficients would be algebraic over $\mathbb F_p$, being symmetric functions of constant algebraic roots. A [rational function](../../../../../rational-function.md) algebraic over $\mathbb F_p$ is constant, so those coefficients would lie in $\mathbb F_p$, contradicting the original irreducibility. The [polynomial](../../../../../polynomial-split.md) $X^p-t$ is irreducible by [Eisenstein criterion](../../../../../eisenstein-criterion.md) at $t$ in $\mathbb F_p[t]$. Both degrees are $p$, but

$$
K(\alpha)=\mathbb F_{p^p}(t),\qquad K(\beta)=\mathbb F_p(\beta).
$$

The first field has $p^p$ roots of $X^{p^p}-X$; the second has only $p$. Indeed a [rational function](../../../../../rational-function.md) algebraic over a finite constant field must be constant: a nonconstant [rational function](../../../../../rational-function.md) makes the transcendental variable algebraic over its own rational-function field, and therefore cannot itself be algebraic over the constants. The root counts are isomorphism invariants. **These extensions are not isomorphic.**

If $K=\mathbb F_q$ is finite, every degree-$d$ extension is a field with $q^d$ elements. Such fields are splitting fields of $X^{q^d}-X$ over $K$, so uniqueness of the [splitting field](../../../../../splitting-field.md) gives a [K-isomorphism](../../../../../k-isomorphism.md). **There is no finite-base-field example of this kind.**

## ↑ Ancestors (10)

1. [18H](../18h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
