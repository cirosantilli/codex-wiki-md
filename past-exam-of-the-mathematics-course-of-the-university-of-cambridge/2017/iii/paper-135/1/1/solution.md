<h1 id="1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $\operatorname{Inj}({<}\omega,X)$ denote the [finite repetition-free sequences](../../../../../../finite-repetition-free-sequence.md), including the empty [sequence](../../../../../../sequence.md). The map $x\mapsto(x)$ is injective, so this [set](../../../../../../set-split.md) is infinite when $X$ is infinite. Suppose, for a contradiction, that it contains a countably infinite subset. Fix its given injective enumeration $s_0,s_1,\ldots$; this is part of the supposition, not a choice from a family of [sets](../../../../../../set-split.md).

Enumerate all pairs $(n,j)$ with $j<\operatorname{length}(s_n)$ by their natural-number pairing codes, recording the corresponding entries $s_n(j)$. If the union of entries were infinite, recursively selecting the first new entry would give an injection $\mathbb N\to X$, contradicting Dedekind-finiteness. Therefore the union is a [finite set](../../../../../../finite-set.md) $F$, say of size $m$. A repetition-free [sequence](../../../../../../sequence.md) over $F$ has length at most $m$, and there are exactly

$$
\sum_{k=0}^m m(m-1)\cdots(m-k+1)=\sum_{k=0}^m\frac{m!}{(m-k)!}
$$

such [sequences](../../../../../../sequence.md), with the empty product equal to one. All $s_n$ would belong to this [finite set](../../../../../../finite-set.md), contradicting their distinctness. Finite counting and the least-code construction use no [axiom of choice](../../../../../../axiom-of-choice.md). This proves [finite repetition-free sequences preserve Dedekind-finiteness](../../../../../../finite-repetition-free-sequences-preserve-dedekind-finiteness.md) and the required infinitude:

$$
\boxed{\operatorname{Inj}({<}\omega,X)\text{ is an infinite Dedekind-finite set.}}
$$

## ↑ Ancestors (11)

1. [1](../1.md)
2. [1](../../1.md)
3. [Paper 135](../../../paper-135-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
