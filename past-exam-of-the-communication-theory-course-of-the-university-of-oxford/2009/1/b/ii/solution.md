<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [chain rule for entropy](../../../../../chain-rule-for-conditional-entropy.md), with $X_r$ placed last, gives

$$
H_n=H(X_{-r})+H(X_r\mid X_{-r}).
$$

Since $X_{-r}$ includes all the preceding coordinates, conditioning monotonicity gives

$$
H(X_r\mid X_{-r})\leq H(X_r\mid X_1,\ldots,X_{r-1}).
$$

This proves the first assertion for every $r$, including $r=1$. Sum over $r$: the conditional terms on the right sum to $H_n$ by the ordinary chain rule. Thus

$$
nH_n\leq\sum_rH(X_{-r})+H_n,
\qquad
\boxed{H_n\leq\frac1{n-1}\sum_rH(X_{-r})}.
$$

This is [Han's entropy inequality](../../../../../han-s-entropy-inequality.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
