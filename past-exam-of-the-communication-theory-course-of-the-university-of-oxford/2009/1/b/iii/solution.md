<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For each $r$, conditioning on all the other coordinates gives no greater [conditional entropy](../../../../../conditional-entropy.md) than conditioning only on the preceding ones. Summing and using the [chain rule for entropy](../../../../../chain-rule-for-conditional-entropy.md) gives directly

$$
\boxed{\sum_rH(X_r\mid X_{-r})\leq\sum_rH(X_r\mid X_1,\ldots,X_{r-1})=H_n}.
$$

Equivalently, the left side is $nH_n-\sum_rH(X_{-r})$, so the same conclusion follows from [Han's entropy inequality](../../../../../han-s-entropy-inequality.md). The direct proof also covers $n=1$, interpreting conditioning on an empty vector as no conditioning.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the communication Theory course of the University of Oxford](../../../../split.md)
6. [Communication Theory course of the University of Oxford](../../../../../communication-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
