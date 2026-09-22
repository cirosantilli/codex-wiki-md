<h1 id="26k/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the buyer's [utility indifference price](../../../../../../indifference-price.md): $\pi(Y)$ is the cash payment satisfying

$$
\sup_{X\in V}\mathbb E U(w_0+X)
=\sup_{X\in V}\mathbb E U(w_0-\pi(Y)+X+Y).
$$

Assume the utilities are well-defined, the finite indifference price exists, and the suprema are attained as allowed. Write the common reference value as $M$. For claims $Y_1,Y_2$, choose optimizers $X_1,X_2$ at their indifference prices $p_1,p_2$. Because $V$ is a [vector space](../../../../../../vector-space-split.md), $X=\theta X_1+(1-\theta)X_2$ is admissible. The [concavity](../../../../../../concave-function.md) of $U$ gives

$$
\mathbb E U\big(w_0-[\theta p_1+(1-\theta)p_2]+X+\theta Y_1+(1-\theta)Y_2\big)\geq\theta M+(1-\theta)M=M.
$$

The optimized utility decreases with the payment; strict increase of $U$ and attainment make the comparison strict whenever a smaller payment is substituted into an attained optimizer. Hence the payment restoring utility $M$ is at least $\theta p_1+(1-\theta)p_2$. Thus

$$
\boxed{\pi(\theta Y_1+(1-\theta)Y_2)\geq\theta\pi(Y_1)+(1-\theta)\pi(Y_2).}
$$

The sign corresponds to buying the payoff. A seller's price uses a different convention.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [26K](../../26k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
