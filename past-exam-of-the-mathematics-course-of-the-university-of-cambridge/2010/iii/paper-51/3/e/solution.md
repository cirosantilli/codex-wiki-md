<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Applying the optimal single-copy filter independently gives a random number $M_n$ of exact successful targets with [binomial distribution](../../../../../../binomial-distribution.md)

$$
M_n\sim\operatorname{Bin}(n,s/t),\qquad
\mathbb E M_n=n\frac{s}{t}.
$$

The [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md) gives $M_n/n\to s/t$ in probability. In contrast, collective [entanglement concentration](../../../../../../entanglement-concentration.md) and [entanglement dilution](../../../../../../entanglement-dilution.md) yield asymptotically $n h_2(s)/h_2(t)$ targets with vanishing output error. The improvement is strict, not just nonnegative. Differentiating [binary entropy](../../../../../../binary-entropy.md) gives

$$
\frac{d}{dx}\left(\frac{h_2(x)}x\right)
=\frac{\log_2(1-x)}{x^2}<0\qquad(0<x<1).
$$

Since $s<t$, it follows that

$$
\boxed{\frac{h_2(s)}{h_2(t)}>\frac{s}{t},\qquad
m(n)\sim n\frac{h_2(s)}{h_2(t)}>\mathbb E M_n.}
$$

This is [collective advantage over independent two-qubit filtering](../../../../../../collective-advantage-over-independent-two-qubit-filtering.md). Independent filtering discards the entanglement in product-state failure branches; the collective reversible asymptotic procedure avoids that extensive loss. The separately filtered targets are exact conditional on success, whereas the collective statement uses the vanishing-error convention from the previous part. Here the counted outputs are target states $|\phi\rangle$; that is also the notation in the original printed question.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
