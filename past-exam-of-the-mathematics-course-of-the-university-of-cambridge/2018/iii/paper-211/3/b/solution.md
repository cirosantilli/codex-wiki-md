<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [time-homogeneous Markov property](../../../../../../time-homogeneous-markov-property.md) and define backward effective parameters by

$$
q_t=\theta_t,\qquad q_j=\theta_j+A(q_{j+1})\quad(j=t-1,\ldots,1).
$$

Conditioning the last exponential factor on $\mathcal F_{t-1}$ replaces $\theta_tX_t$ by $A(q_t)X_{t-1}+B(q_t)$. Repeating the [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) combines this with the preceding exponent, then with each earlier exponent. The last remaining conditional transform is at time $1$, so

$$
\boxed{A_t(\theta_1,\ldots,\theta_t)=A(q_1),\qquad B_t(\theta_1,\ldots,\theta_t)=\sum_{j=1}^t B(q_j).}
$$

These are finite because the one-step [affine process](../../../../../../affine-process.md) transforms are finite at every real parameter. The argument establishes the entire [joint affine transform](../../../../../../joint-affine-transform.md), including when the coefficients $\theta_j$ have different signs.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
