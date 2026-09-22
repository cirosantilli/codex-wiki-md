<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Factor the first characteristic polynomial:

$$
\rho(\zeta)=(\zeta-1)(\zeta-5/7).
$$

The unit root is simple and the other root is strictly inside the unit disk, so the method is [zero-stable](../../../../../../zero-stability.md). Also $\rho(1)=0$ and $\rho'(1)=\sigma(1)=2/7$, giving [numerical consistency](../../../../../../consistency-of-a-numerical-method.md). The [Dahlquist equivalence theorem](../../../../../../dahlquist-equivalence-theorem.md) therefore makes it convergent.

The mechanism can also be seen directly. The [zero-stable](../../../../../../zero-stability.md) homogeneous recurrence has bounded propagators because its two error modes are $1$ and $(5/7)^n$. Variation of constants for the perturbed recurrence bounds the error by a fixed multiple of its two starting errors and the sum of the step defects, plus $O(h)$ times a sum of errors from the Lipschitz vector field. Absorb the current implicit error term for sufficiently small $h$, then apply the [discrete Gronwall inequality](../../../../../../discrete-gronwall-inequality.md). On a fixed time interval the sum of $O(h^3)$ exact-start defects is $O(h^2)$, giving **second-order [numerical convergence](../../../../../../convergence-of-a-numerical-method.md) with second-order starting values**. The implicit step is locally well defined, for example by contraction when $4hL/7<1$ for a [Lipschitz constant](../../../../../../lipschitz-constant.md) $L$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
