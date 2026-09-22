<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Itô formula](../../../../../../ito-s-lemma.md) verifies the [geometric Brownian motion](../../../../../../geometric-brownian-motion.md) solution

$$
X_t=x\exp\!\left((b-\tfrac12\sigma^2)t+\sigma B_t\right).
$$

This is valid for negative $x$ as well as positive $x$; $x=0$ gives the zero solution. [Pathwise uniqueness](../../../../../../pathwise-uniqueness.md) follows from the [Lipschitz continuity](../../../../../../lipschitz-continuity.md) of the linear coefficients. The [moment-generating function of a normal distribution](../../../../../../moment-generating-function-of-a-normal-distribution.md) gives $\mathbb Ee^{k\sigma B_t}=e^{k^2\sigma^2t/2}$, and therefore

$$
\boxed{\mathbb E(X_t^k)=x^k\exp\!\left(\left(kb+\frac{k(k-1)}2\sigma^2\right)t\right)\qquad(k\geq1).}
$$

These [moments](../../../../../../moment.md) are finite on every finite horizon. If the convention $0\in\mathbb N$ is used, the zeroth [moment](../../../../../../moment.md) is $1$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
