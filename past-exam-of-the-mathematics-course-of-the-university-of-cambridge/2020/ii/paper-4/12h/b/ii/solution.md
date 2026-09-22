<h1 id="12h/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose $a_j\leq A$ for every $j$. Given $b>0$, choose the first convergent denominator $q_m\geq b$. Then $q_{m-1}<b$ and the recurrence gives $q_m=a_mq_{m-1}+q_{m-2}<(A+1)b$. Part (i), applied at index $m$, gives $|b\alpha-a|\geq|q_m\alpha-p_m|$.

If $\alpha_{m+1}=[a_{m+1};a_{m+2},\ldots]$ is the complete quotient, the exact error formula is

$$
|q_m\alpha-p_m|
=\frac1{q_m\alpha_{m+1}+q_{m-1}}.
$$

Since $\alpha_{m+1}<A+1$, this is greater than $1/((A+2)q_m)$ and therefore greater than $1/((A+1)(A+2)b)$. It follows that every rational $a/b$ satisfies

$$
\left|\alpha-\frac ab\right|>
\frac1{(A+1)(A+2)b^2}.
$$

**Thus one may take $c=((A+1)(A+2))^{-1}$.**

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [12H](../../../12h.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
