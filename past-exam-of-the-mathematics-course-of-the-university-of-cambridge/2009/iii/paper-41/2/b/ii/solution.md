<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume that, conditional on the recorded embarrassment category, answering the item is independent of virginity status. Also assume that this category is assessed comparably for both groups and that both response strata have positive observation probabilities. This is [covariate-dependent missing completely at random](../../../../../../../covariate-dependent-missing-completely-at-random.md) for the item response with embarrassment as the fully observed [covariate](../../../../../../../covariate.md); it supports [MAR standardization over a fully observed covariate](../../../../../../../mar-standardization-over-a-fully-observed-covariate.md).

Use the responder probabilities $0.18$ and $0.08$ within strata, but the [stratum](../../../../../../../stratum.md) sizes in the full group of responders plus item nonresponders: $300$ and $450$. This gives

$$
\boxed{\widehat p_{R+I}=\frac{300(0.18)+450(0.08)}{750}
=\frac{90}{750}=12\%.}
$$

Equivalently, the estimated missing positive counts are $100(0.18)=18$ and $50(0.08)=4$, adding 22 to the 68 observed positives. The marginal estimate changes because the full group contains a larger proportion judged embarrassed. Merely copying the unstratified responder percentage would ignore that difference. The [conditional independence](../../../../../../../conditional-independence.md) assumption cannot be verified using the missing item responses.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 41](../../../../paper-41-split.md)
5. [Iii](../../../../split.md)
6. [2009](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
