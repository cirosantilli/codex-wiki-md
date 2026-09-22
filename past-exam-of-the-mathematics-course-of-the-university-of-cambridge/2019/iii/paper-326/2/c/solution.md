<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The assumptions prove convergence to the set of [J-minimizing solutions](../../../../../../j-minimizing-solution.md), and subsequential convergence to a member of that set. Convergence to a single fixed member requires uniqueness or a suitable selection rule.

Let $u^\dagger$ be any [J-minimizing solution](../../../../../../j-minimizing-solution.md), whose existence is granted. It is feasible for every noisy-data constraint because $Au^\dagger=f$ and $\|f-f_\delta\|\leq\delta$. Minimality therefore gives $J(u_\delta)\leq J(u^\dagger)$. All reconstructions lie in this strongly [sequentially compact space](../../../../../../sequentially-compact-space.md) sublevel set. For any sequence $\delta_k\downarrow0$, pass to a subsequence with $u_{\delta_k}\to u_*$. Boundedness of $A$ and the [triangle inequality](../../../../../../triangle-inequality.md) imply

$$
\|Au_{\delta_k}-f\|\leq\|Au_{\delta_k}-f_{\delta_k}\|+\|f_{\delta_k}-f\|\leq2\delta_k,
$$

so $Au_*=f$. By [sequential lower semicontinuity](../../../../../../sequential-lower-semicontinuity.md),

$$
J(u_*)\leq\liminf_k J(u_{\delta_k})\leq J(u^\dagger).
$$

Thus $u_*$ is a [J-minimizing solution](../../../../../../j-minimizing-solution.md). The same compactness argument shows the [distance to a set](../../../../../../distance-to-a-set.md) of exact minimizers tends to zero: otherwise a subsequence at a fixed positive distance would converge to an exact minimizer, a contradiction. If that minimizer is unique, every convergent subsequence has the same limit, giving the asserted full [strong convergence](../../../../../../norm-convergence.md).

For a counterexample to full convergence under the printed hypotheses alone, take $\mathcal U=\mathcal V=\mathbb R$, $A=0$, $f=f_\delta=0$, and $J(u)=\max\{|u|-1,0\}$. This is nonnegative and continuous, with compact sublevel sets $[-1-C,1+C]$ for $C\geq0$. Every point of $[-1,1]$ is both an exact and a residual-method minimizer. Choosing $u_{1/k}=(-1)^k$ gives a valid sequence of minimizers that does not converge. The reusable corrected statement is [compact-sublevel convergence of the residual method](../../../../../../compact-sublevel-convergence-of-the-residual-method.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
