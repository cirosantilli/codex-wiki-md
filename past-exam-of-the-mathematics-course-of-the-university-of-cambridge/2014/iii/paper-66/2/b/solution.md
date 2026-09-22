<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Dahlquist equivalence theorem](../../../../../../dahlquist-equivalence-theorem.md) states that a consistent [linear multistep method](../../../../../../linear-multistep-method.md) is convergent for suitably consistent starting values exactly when it is [zero-stable](../../../../../../zero-stability.md). The [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) requires every root of $\rho$ to lie in the closed unit disk, with every unit-modulus root simple.

The roots are $1$ and $a$. Thus $|a|\leq1$ is necessary; $a=1$ is excluded because it gives a double root at one. At $a=-1$, the two unit roots are distinct, so the endpoint is allowed. Combined with part (a), this proves

$$
\boxed{-1\leq a<1\quad\text{for convergence}.}
$$

Assume a locally Lipschitz vector field, a smooth solution on the fixed time interval, a nearby solvable implicit branch and starting errors of the required order. The global order is three at $a=-1/5$ and two at the other convergent parameter values. Outside this interval, zero-step perturbations already grow through either an exterior root or a unit-root polynomial factor.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
