<h1 id="a/3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [unilateral shift operator](../../../../../unilateral-shift-operator.md) $R$ is not onto, since its outputs have first coordinate zero. The [left shift operator](../../../../../left-shift-operator.md) $L$ is not injective, since $Le_1=0$. Both have [operator norm](../../../../../operator-norm.md) one, and $LR=I$. Consequently

$$
L(R+A)=LR+LA=I+LA.
$$

If $\|A\|<1$, then $\|LA\|<1$, so the [Neumann series](../../../../../neumann-series.md) makes $I+LA$ invertible. If $R+A$ were invertible too, the identity above would give

$$
L=(I+LA)(R+A)^{-1},
$$

a product of invertible operators, contradicting the nontrivial [kernel](../../../../../kernel-of-a-linear-map-split.md) of $L$. Thus

$$
\boxed{\|A\|<1\Longrightarrow R+A\text{ is not invertible}.}
$$

This is [norm stability of noninvertibility for the unilateral right shift](../../../../../norm-stability-of-noninvertibility-for-the-unilateral-right-shift.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the analysis course of the University of Oxford](../../../../split.md)
6. [Analysis course of the University of Oxford](../../../../../analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
