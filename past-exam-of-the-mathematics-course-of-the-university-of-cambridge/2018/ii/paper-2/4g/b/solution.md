<h1 id="4g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\widehat\delta_E(q_0,w)$ mean all states reachable after reading $w$, allowing arbitrary epsilon transitions before, between, and after its symbols. We prove by [mathematical induction](../../../../../../mathematical-induction.md) on $|w|$ that

$$
\widehat\delta_E(q_0,w)=\widehat\delta_D(q_D,w).
$$

For $w=\epsilon$, both sides equal $E(\{q_0\})=q_D$. Suppose the claim holds for $w$, and append $a\in\Sigma$. By the definitions of the extended transition functions and the subset construction,

$$
\widehat\delta_E(q_0,wa)
=E\bigl(\delta_E(\widehat\delta_E(q_0,w),a)\bigr)
=\delta_D(\widehat\delta_D(q_D,w),a)
=\widehat\delta_D(q_D,wa).
$$

This completes the induction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4G](../../4g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
