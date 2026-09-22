<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a fixed-step [linear multistep method](../../../../../../linear-multistep-method.md) with a nonzero leading coefficient, applied to an [ordinary differential equation](../../../../../../ordinary-differential-equation.md) with a locally [Lipschitz continuous](../../../../../../lipschitz-continuity.md) vector field, the [Dahlquist equivalence theorem](../../../../../../dahlquist-equivalence-theorem.md) states that

$$
\boxed{\text{convergence}\ \Longleftrightarrow\
\text{consistency and zero-stability}.}
$$

Here convergence is uniform on each fixed finite time interval as the [step size](../../../../../../step-size.md) tends to zero, for every set of starting values tending to the corresponding exact values. [Consistency of a numerical method](../../../../../../consistency-of-a-numerical-method.md) means that the normalized local defect tends to zero; for the [characteristic polynomials of a linear multistep method](../../../../../../characteristic-polynomials-of-a-linear-multistep-method.md) it gives $\rho(1)=0$ and $\rho'(1)=\sigma(1)$. [Zero-stability](../../../../../../zero-stability.md) is equivalent to the [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md): every [root of a polynomial](../../../../../../root-of-a-polynomial.md) $\xi$ of $\rho$ satisfies $|\xi|\leq1$, and roots with $|\xi|=1$ are simple. Order $p\geq1$, together with [zero-stability](../../../../../../zero-stability.md) and starting errors $O(h^p)$, gives [global error](../../../../../../global-discretization-error.md) $O(h^p)$ under the usual smoothness assumptions.

To prove the [necessity of the root condition for multistep convergence](../../../../../../necessity-of-the-root-condition-for-multistep-convergence.md), use the test problem $y'=0$, $y(0)=0$. Its discrete error satisfies $\rho(E)e_n=0$, where $Ee_n=e_{n+1}$. Set $h=T/N$. If $|\xi|>1$, the exact recurrence solution

$$
e_n=|\xi|^{-N}\xi^n
$$

has starting errors tending to zero at every fixed starting index, but $|e_N|=1$. Thus convergence fails.

If a unit-modulus root has multiplicity $m\geq2$, the recurrence instead admits

$$
e_n=N^{-(m-1)}n^{m-1}\xi^n.
$$

Again every fixed starting error tends to zero while $|e_N|=1$. These polynomial-times-exponential solutions follow from the repeated factor $(E-\xi)^m$. Complex modes can be interpreted as a real two-component system, or their real and imaginary parts can be used. Therefore **convergence requires precisely the [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md)**. Repeated roots strictly inside the unit disk are allowed, since their polynomial factors are dominated by exponential decay.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
