<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Interpret the printed missing parenthesis as ending $f(y_{n+2})$ before the next summand. The [characteristic polynomials of a linear multistep method](../../../../../characteristic-polynomials-of-a-linear-multistep-method.md) are then

$$
\rho(\zeta)=\zeta^3-(1+2\alpha)\zeta^2+(1+2\alpha)\zeta-1
=(\zeta-1)(\zeta^2-2\alpha\zeta+1),
$$



$$
\sigma(\zeta)=\frac\zeta6[(5+\alpha)\zeta^2-(4+8\alpha)\zeta+11-5\alpha].
$$

They satisfy $\rho(1)=0$ and $\rho'(1)=\sigma(1)=2(1-\alpha)$, so the consistency identities hold. The two nonprincipal roots are reciprocal. If $|\alpha|<1$, they are $\alpha\pm i\sqrt{1-\alpha^2}$, distinct unit roots also distinct from the principal root one. If $|\alpha|>1$, one reciprocal root lies outside the unit circle. At $\alpha=1$ the root one is triple, and at $\alpha=-1$ the root minus one is double. The [root condition for a multistep method](../../../../../root-condition-for-a-multistep-method.md) therefore holds exactly when $-1<\alpha<1$. The [Dahlquist equivalence theorem](../../../../../dahlquist-equivalence-theorem.md), with standard smoothness and consistent starting data, gives

$$
\boxed{\text{Convergent exactly for }-1<\alpha<1.}
$$

To determine order rather than guess it from the number of steps, the [exponential-symbol order criterion for a multistep method](../../../../../exponential-symbol-order-criterion-for-a-multistep-method.md) gives

$$
\rho(e^z)-z\sigma(e^z)=-\frac{\alpha+5}{12}z^4-\frac{14\alpha+61}{90}z^5+O(z^6).
$$

Thus **the formal order is three for $\alpha\ne-5$, and four for $\alpha=-5$**. At the exceptional value the $z^5$ coefficient is $1/10$. That fourth-order formula is not zero-stable. Every convergent member consequently has global order three. At $\alpha=1$ the third-order Taylor cancellation is only a formal defect property of a degenerate, nonconvergent recurrence.

Here is a direct [A-stability](../../../../../a-stability.md) test for the convergent parameters. For a nonprincipal unit root $r=\alpha+i\sqrt{1-\alpha^2}$, the simple root of the [amplification polynomial of a multistep method](../../../../../amplification-polynomial-of-a-multistep-method.md) satisfies

$$
r(z)=r+z\frac{\sigma(r)}{\rho'(r)}+O(z^2).
$$

Reduction using $r^2-2\alpha r+1=0$ gives

$$
\frac{\sigma(r)}{r\rho'(r)}=
\frac{2\alpha^2r+4\alpha r-\alpha-3r-2}{6[(2\alpha+1)r-1]},\qquad
\operatorname{Re}\frac{\sigma(r)}{r\rho'(r)}=\frac{\alpha-1}{12}<0.
$$

For small negative real $z$, it follows that

$$
|r(z)|^2=1+\frac{\alpha-1}{6}z+O(z^2)>1.
$$

So even a small negative real test parameter has an amplifying parasitic mode. **None of the convergent parameters is A-stable.** Parameters outside this range already fail the necessary zero-step root condition, so **there is no real $\alpha$ giving an A-stable original method**.

The endpoint $\alpha=1$ is worth keeping separate from a misleading cancellation: there $\rho=(\zeta-1)^3$ and $\sigma=\zeta(\zeta-1)^2$. The original amplification polynomial retains the double root one for every $z$, giving unbounded polynomial parasitic modes for general starting values. Canceling $(\zeta-1)^2$ would yield a different, reduced [Backward Euler method](../../../../../backward-euler-method.md); it does not stabilize the original recurrence. This is the [common-factor cancellation defect in a multistep recurrence](../../../../../common-factor-cancellation-defect-in-a-multistep-recurrence.md). The family is summarized by the [reciprocal-root three-step multistep family](../../../../../reciprocal-root-three-step-multistep-family.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
