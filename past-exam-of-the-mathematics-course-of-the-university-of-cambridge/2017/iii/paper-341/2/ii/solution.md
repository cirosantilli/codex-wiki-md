<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The first [characteristic polynomials of a linear multistep method](../../../../../../characteristic-polynomials-of-a-linear-multistep-method.md) is

$$
\rho(\zeta)=\zeta^2-(1+\alpha)\zeta+\alpha=(\zeta-1)(\zeta-\alpha).
$$

The [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) requires $|\alpha|\leq1$ and excludes $\alpha=1$, where the [root of a polynomial](../../../../../../root-of-a-polynomial.md) at one is double. At $\alpha=-1$, the two unit-modulus [roots of a polynomial](../../../../../../root-of-a-polynomial.md) are distinct, so [zero-stability](../../../../../../zero-stability.md) holds. For $\alpha\ne1$, the first-order [consistency of a numerical method](../../../../../../consistency-of-a-numerical-method.md) identity is $\rho'(1)=1-\alpha$, equal to the coefficient of $hf$.

Using the permitted [Dahlquist equivalence theorem](../../../../../../dahlquist-equivalence-theorem.md) in this [multiderivative multistep method](../../../../../../multiderivative-multistep-method.md) setting gives

$$
\boxed{-1\leq\alpha<1}.
$$

This means convergence on every fixed finite time interval where the smooth exact [solution of a differential equation](../../../../../../solution-of-a-differential-equation.md) exists, with consistent starting values and the nearby branch of each implicit solve. More specifically, the [convergence of a zero-stable multiderivative method](../../../../../../convergence-of-a-zero-stable-multiderivative-method.md) gives order $p$ when the starting errors are $O(h^p)$ and both $f$ and $f'f$ are locally uniformly [Lipschitz continuous](../../../../../../lipschitz-continuity.md) on the relevant region.

The exclusions are genuine. For $y'=0$ and $|\alpha|>1$, an arbitrarily small parasitic starting error is amplified as $\alpha^n$. At $\alpha=1$, take $y_0=0$, $y_1=h$, also for $y'=0$. The exact solution is zero, but the numerical recurrence gives $y_n=nh$, an error of order one at fixed positive time. This proves failure even though the starting values converge.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
