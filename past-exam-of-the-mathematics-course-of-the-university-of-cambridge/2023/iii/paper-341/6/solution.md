<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A linear [multistep method](../../../../../linear-multistep-method.md) for $y'=f(t,y)$ has the form

$$
\sum_{j=0}^s\alpha_jy_{n+j}
=h\sum_{j=0}^s\beta_jf_{n+j},
\qquad \alpha_s=1.
$$

Its [characteristic polynomials of a linear multistep method](../../../../../characteristic-polynomials-of-a-linear-multistep-method.md) are $\rho(\zeta)=\sum_j\alpha_j\zeta^j$ and $\sigma(\zeta)=\sum_j\beta_j\zeta^j$. Substitution of the exact solution, or equivalently expansion of $\rho(e^z)-z\sigma(e^z)$ at $z=0$, gives the [order conditions for a linear multistep method](../../../../../order-conditions-for-a-linear-multistep-method.md). The method has order $p$ when

$$
\rho(e^z)-z\sigma(e^z)=O(z^{p+1}),
$$

with a nonzero coefficient at the next power. Its one-step defect is then $O(h^{p+1})$, while its global error is $O(h^p)$ when stability prevents accumulation from being amplified.

Order alone does not ensure convergence because the recurrence may contain growing parasitic modes. [Zero-stability](../../../../../zero-stability.md) is the [root condition for a multistep method](../../../../../root-condition-for-a-multistep-method.md): every root of $\rho$ lies in $|\zeta|\leq1$, and every root on the unit circle is simple. Consistency is the first-order condition

$$
\rho(1)=0,
\qquad
\rho'(1)=\sigma(1).
$$

The [Dahlquist equivalence theorem](../../../../../dahlquist-equivalence-theorem.md) states that a consistent linear multistep method is convergent if and only if it is zero-stable. For example, the leapfrog method $y_{n+2}-y_n=2hf_{n+1}$ has $\rho(\zeta)=\zeta^2-1$; its roots $\pm1$ are simple, so this second-order method is convergent, although its parasitic $-1$ mode can oscillate.

To study stiff decay, apply the method to $y'=\lambda y$ and put $z=h\lambda$. The amplification factors are the roots of

$$
\rho(\zeta)-z\sigma(\zeta)=0.
$$

The [linear stability domain](../../../../../linear-stability-domain.md) consists of the $z$ for which these roots satisfy the strict interior condition appropriate away from the boundary, with simple unit roots where boundary stability is admitted. The method is [A-stable](../../../../../a-stability.md) when this domain contains the left half-plane, so every mode with $\operatorname{Re}\lambda<0$ remains bounded for every positive step size. The [Second Dahlquist barrier](../../../../../second-dahlquist-barrier.md) says that an A-stable multistep method has order at most two.

The main families illustrate the tradeoffs. The explicit Adams-Bashforth methods interpolate past derivative values and are inexpensive, but their stability domains are bounded. The implicit Adams-Moulton methods include the new derivative value; the one-step second-order member is the [trapezoidal rule](../../../../../trapezoidal-rule.md), which is A-stable. The backward differentiation formulas interpolate past solution values and differentiate the interpolant; the first two are A-stable, while higher orders retain useful sectors of the left half-plane. Implicit methods require a nonlinear solve at each step, commonly initialized by an explicit predictor to form a predictor-corrector pair. Thus order controls consistency error, the root condition controls convergence as $h\to0$, and the amplification polynomial controls whether a convergent method remains useful on stiff equations.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 341](../../paper-341-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
