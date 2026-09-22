<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $Y=g(S)$ and $Z=\min(S,M)$. Their common [expected value](../../../../../../expected-value.md) is $c$. Expanding about the retention gives **the requested variance identity**

$$
\mathbb E[(Y-M)^2]-(M-c)^2
=\mathbb E[Y^2]-2Mc+M^2-(M^2-2Mc+c^2)
=\boxed{\operatorname{Var}(Y)}.
$$

The [stop loss variance minimization principle](../../../../../../stop-loss-variance-minimization-principle.md) follows from a pointwise comparison. For $0\leq x\leq M$, the constraint $0\leq g(x)\leq x$ implies

$$
|g(x)-M|=M-g(x)\geq M-x
=|\min(x,M)-M|.
$$

For $x>M$, the squared distance of $\min(x,M)=M$ from $M$ is zero, so the same squared-distance comparison is immediate. Therefore

$$
\mathbb E[(Y-M)^2]\geq\mathbb E[(Z-M)^2].
$$

Subtracting the same $(M-c)^2$ proves **optimality of the retained stop loss payout**:

$$
\boxed{\operatorname{Var}(g(S))\geq
\operatorname{Var}(\min(S,M)).}
$$

Since $Z$ is bounded, its [variance](../../../../../../variance-split.md) is finite; if $\mathbb E[Y^2]=\infty$, the inequality remains valid with infinite [variance](../../../../../../variance-split.md) on the left. When it is finite, equality requires $g(S)=\min(S,M)$ almost surely, because the pointwise squared-distance inequality is strict whenever the two payouts differ.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
