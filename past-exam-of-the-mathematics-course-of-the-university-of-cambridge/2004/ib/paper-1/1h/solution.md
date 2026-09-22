<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

Expand $e_{r+1}$ in the given [spanning set](../../../../../spanning-set.md):

$$
e_{r+1}=\sum_{i=1}^ra_ie_i+\sum_{j=r+1}^mb_jf_j.
$$

Some $b_j$ must be nonzero, since otherwise $e_{r+1}$ would lie in the span of the earlier $e_i$, contradicting [linear independence](../../../../../linear-independence.md). Reorder the remaining $f_j$ so $b_{r+1}\ne0$. Solving this equation for $f_{r+1}$ expresses it in terms of $e_1,\ldots,e_{r+1},f_{r+2},\ldots,f_m$. Every member of the old [spanning set](../../../../../spanning-set.md) is therefore in the new span, so **the replacement set still spans $V$**. This proves the needed step of the [Steinitz exchange lemma](../../../../../steinitz-exchange-lemma.md) directly.

Starting with $f_1,\ldots,f_m$, apply that replacement successively to $e_1,e_2,\ldots$. After $r\leq m$ steps the spanning list is $e_1,\ldots,e_r$ together with $m-r$ unreplaced $f$'s. If $n>m$, after $m$ replacements the list $e_1,\ldots,e_m$ spans $V$, forcing $e_{m+1}$ to be a [linear combination](../../../../../linear-combination.md) of it. That contradicts [linear independence](../../../../../linear-independence.md). Hence **$\boxed{n\leq m}$**.

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
