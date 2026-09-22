<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The first [characteristic polynomial](../../../../../../characteristic-polynomial.md) factors as

$$
\rho(w)=(w-1)(w^2-2\alpha w+1).
$$

Also $\rho(1)=0$ and $\rho'(1)=\sigma(1)=2(1-\alpha)$, so the [order conditions for a linear multistep method](../../../../../../order-conditions-for-a-linear-multistep-method.md) hold for every $\alpha$. Convergence of the full [linear multistep method](../../../../../../linear-multistep-method.md) recurrence requires, in addition, the [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md): all [polynomial roots](../../../../../../root-of-a-polynomial.md) of $\rho$ lie in the closed unit disk and its [polynomial roots](../../../../../../root-of-a-polynomial.md) on the unit circle are simple.

For $-1<\alpha<1$, write $\alpha=\cos\theta$ with $0<\theta<\pi$. The other [polynomial roots](../../../../../../root-of-a-polynomial.md) are $e^{\pm i\theta}$, distinct from each other and from 1, so the [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) holds. For $|\alpha|>1$, the two quadratic [polynomial roots](../../../../../../root-of-a-polynomial.md) are real and reciprocal, and one has modulus greater than one. At $\alpha=1$, $\rho=(w-1)^3$; at $\alpha=-1$, $\rho=(w-1)(w+1)^2$. Both endpoints violate simplicity. [Consistency of a numerical method](../../../../../../consistency-of-a-numerical-method.md) plus [zero-stability](../../../../../../zero-stability.md) therefore gives

$$
\boxed{-1<\alpha<1.}
$$

The conclusion applies to the recurrence as printed, including its starting data. Canceling common factors is not innocuous: at $\alpha=1$ the [polynomials](../../../../../../polynomial-split.md) contain $(w-1)^2$, and at $\alpha=-13/5$ they contain $w+5$. The reduced recurrences exclude parasitic solutions of the original one. This is the [common-factor cancellation defect in a multistep recurrence](../../../../../../common-factor-cancellation-defect-in-a-multistep-recurrence.md), so those parameter values are not added to the interval.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
