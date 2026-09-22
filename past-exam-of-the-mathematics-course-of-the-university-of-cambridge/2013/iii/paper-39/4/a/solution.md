<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Backward induction makes the [Snell envelope](../../../../../../snell-envelope.md) integrable and adapted: $|U_t|\le|Y_t|+\mathbb E(|U_{t+1}|\mid\mathcal F_t)$. Its definition gives $U_t\ge Y_t$ and $U_t\ge\mathbb E(U_{t+1}\mid\mathcal F_t)$, so it is a [supermartingale](../../../../../../supermartingale.md) dominating the reward.

For a [stopping time](../../../../../../stopping-time.md) $\tau$ taking values in $\{0,\ldots,T\}$, expand its stopped value as

$$
U_\tau=U_0+\sum_{t=0}^{T-1}\mathbf1_{\{\tau>t\}}(U_{t+1}-U_t).
$$

The indicators are $\mathcal F_t$-measurable. Taking [conditional expectations](../../../../../../conditional-expectation.md) in each summand makes its expectation nonpositive by the [supermartingale](../../../../../../supermartingale.md) property. Since $\mathcal F_0$ is trivial, $U_0$ is deterministic and

$$
\boxed{\mathbb E Y_\tau\le\mathbb E U_\tau\le U_0.}
$$

This proves the finite-horizon [optional sampling theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) directly in the instance needed here, without assuming nonnegative rewards.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
