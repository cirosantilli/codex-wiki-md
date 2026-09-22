<h1 id="b/5/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

By the [natural-number recursion theorem](../../../../../../natural-number-recursion-theorem.md), let $\alpha_0=0$ and $\alpha_{n+1}=F(\alpha_n)$. These [ordinals](../../../../../../ordinal-split.md) form a nondecreasing sequence by the preceding bound. If $\alpha_{n+1}=\alpha_n$ for some $n$, it is already a fixed point.

Otherwise the sequence is strictly increasing. Its supremum $\lambda=\bigcup_{n<\omega}\alpha_n$ is a [limit ordinal](../../../../../../limit-ordinal.md), and the sequence is cofinal in it. Continuity and monotonicity give

$$
F(\lambda)=\sup_{\beta<\lambda}F(\beta)=\sup_{n<\omega}F(\alpha_n)=\sup_{n<\omega}\alpha_{n+1}=\lambda.
$$

For the middle equality, every $\beta<\lambda$ is below some $\alpha_n$, while every $\alpha_n<\lambda$. Therefore **$F$ has a fixed point**. The sequence is a set by [Axiom schema of replacement](../../../../../../axiom-schema-of-replacement.md), since $F$ is a definable [set-theoretic class function](../../../../../../set-theoretic-class-function.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [B](../../../../b.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the logic and set theory course of the University of Oxford](../../../../../split.md)
7. [Logic and set theory course of the University of Oxford](../../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
