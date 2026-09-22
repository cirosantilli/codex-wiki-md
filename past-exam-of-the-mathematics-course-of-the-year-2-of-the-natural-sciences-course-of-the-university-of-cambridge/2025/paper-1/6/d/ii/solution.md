<h1 id="6/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $K(t)=e^{tR}Se^{-tR}$. The [product rule](../../../../../../product-rule.md) and differentiation of the [matrix exponential](../../../../../../matrix-exponential.md) give

$$
K'(t)=RK(t)-K(t)R=[R,K(t)],\qquad K''(t)=[R,[R,K(t)]],
$$

where brackets are the [operator commutator](../../../../../../operator-commutator.md). Evaluating at zero gives $K(0)=S$, $K'(0)=[R,S]$ and $K''(0)=[R,[R,S]]$. The [Taylor series](../../../../../../taylor-series.md) at zero is consequently

$$
\boxed{e^{tR}Se^{-tR}=S+t[R,S]+\frac{t^2}{2}[R,[R,S]]+O(t^3).}
$$

In particular $[R,[R,S]]=R^2S-2RSR+SR^2$, which also follows by multiplying the two [matrix exponential](../../../../../../matrix-exponential.md) series through quadratic order. For fixed finite [matrices](../../../../../../matrix.md) the remainder has the stated [Big O notation](../../../../../../big-o-notation.md) in any [matrix norm](../../../../../../matrix-norm.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [6](../../../6.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
