<h1 id="17c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The first characteristic polynomial of the [linear multistep method](../../../../../../linear-multistep-method.md) comes only from its left side:

$$
\rho(\zeta)=\zeta^2-\zeta=\zeta(\zeta-1).
$$

Its roots are zero and one; both lie in the closed unit disc, and the only unit-modulus root is simple. Thus the method satisfies the [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) and is [zero-stable](../../../../../../zero-stability.md). Part (b) showed consistency for every $\alpha,\beta$. The [Dahlquist equivalence theorem](../../../../../../dahlquist-equivalence-theorem.md) states that a consistent linear multistep method is convergent exactly when it is zero-stable. Therefore

$$
\boxed{\text{the method is convergent}}
$$

under the usual Lipschitz hypotheses on $f$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17C](../../17c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
