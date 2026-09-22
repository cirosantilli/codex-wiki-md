<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Suppose first that $L/K$ is a [totally ramified extension](../../../../../../totally-ramified-extension.md) of degree $n$, and let $\alpha$ be a [uniformizer](../../../../../../uniformizer.md) of $L$. If the valuation on $L$ is normalized by $v_L(\alpha)=1$, then $v_L(K^\times)=n\mathbb Z$. The value group of $K(\alpha)$ already contains both $n\mathbb Z$ and $1$, so its [ramification index](../../../../../../ramification-index.md) over $K$ is at least $n$. Hence $[K(\alpha):K]\geq n$, and therefore $L=K(\alpha)$.

Let

$$
f(X)=X^n+a_{n-1}X^{n-1}+\cdots+a_0
$$

be the [minimal polynomial](../../../../../../minimal-polynomial.md) of $\alpha$. Every conjugate of $\alpha$ has positive valuation, so each $a_i$ lies in the maximal ideal of $\mathcal O_K$. Moreover

$$
v_L(a_0)=v_L\bigl(N_{L/K}(\alpha)\bigr)=n,
$$

which means $v_K(a_0)=1$. Thus $f$ is an [Eisenstein polynomial](../../../../../../eisenstein-polynomial.md).

Conversely, if $\alpha$ is a root of an Eisenstein polynomial of degree $n$, the [Eisenstein criterion](../../../../../../eisenstein-criterion.md) makes that polynomial irreducible and its [Newton polygon](../../../../../../newton-polygon.md) gives $v_L(\alpha)=1/n$ when $v_K$ is normalized. Consequently $e(K(\alpha)/K)\geq n$; equality with the field degree forces $e=n$ and [residue-field degree](../../../../../../residue-field-degree.md) one. Thus $K(\alpha)/K$ is totally ramified.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
