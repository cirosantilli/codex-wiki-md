<h1 id="18d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Dahlquist equivalence theorem](../../../../../../dahlquist-equivalence-theorem.md) states that a [linear multistep method](../../../../../../linear-multistep-method.md) has [convergence of a numerical method](../../../../../../convergence-of-a-numerical-method.md) **if and only if it is consistent and zero-stable**, under the standard assumptions for the [initial value problem](../../../../../../initial-value-problem.md) and convergent starting values. [Consistency of a numerical method](../../../../../../consistency-of-a-numerical-method.md) means order at least one, or

$$
\rho(1)=0,\qquad \rho'(1)=\sigma(1),\quad \rho(\zeta)=\sum_{\ell=0}^s\rho_\ell\zeta^\ell,\quad \sigma(\zeta)=\sum_{\ell=0}^s\sigma_\ell\zeta^\ell.
$$

The [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) expresses [zero-stability](../../../../../../zero-stability.md): every root of $\rho$ has modulus at most one, and every root with modulus one is simple. Usual hypotheses include a well-posed [ordinary differential equation](../../../../../../ordinary-differential-equation.md) with $f$ continuous in time and [Lipschitz continuous](../../../../../../lipschitz-continuity.md) in the solution variable, a valid step equation, and starting approximations converging to the exact values.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18D](../../18d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
