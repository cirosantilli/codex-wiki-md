<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A constant-step [linear multistep method](../../../../../linear-multistep-method.md) has the form

$$
\sum_{j=0}^k\alpha_jY_{n+j}=h\sum_{j=0}^k\beta_jf(t_{n+j},Y_{n+j}),\qquad\rho(\zeta)=\sum_{j=0}^k\alpha_j\zeta^j,\quad\sigma(\zeta)=\sum_{j=0}^k\beta_j\zeta^j,
$$

with $\alpha_k\ne0$. The [characteristic polynomials of a linear multistep method](../../../../../characteristic-polynomials-of-a-linear-multistep-method.md) encode both accuracy and error propagation. The method has [order of a numerical method](../../../../../order-of-a-numerical-method.md) $p$ when insertion of a sufficiently smooth exact solution leaves an unnormalized [local truncation error](../../../../../local-truncation-error.md) $O(h^{p+1})$. The [exponential-symbol order criterion for a multistep method](../../../../../exponential-symbol-order-criterion-for-a-multistep-method.md) expresses this as $\rho(e^z)-z\sigma(e^z)=O(z^{p+1})$. In particular, first-order [consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md) requires $\rho(1)=0$ and $\rho'(1)=\sigma(1)$.

Accuracy alone is insufficient. For $f=0$, perturbations obey the recurrence $\rho(E)e_n=0$. The [root condition for a multistep method](../../../../../root-condition-for-a-multistep-method.md) requires every [root of a polynomial](../../../../../root-of-a-polynomial.md) $\rho$ to lie in the closed [unit disk](../../../../../unit-disk.md), with each [unit-circle root](../../../../../unit-circle-root.md) simple. This is [zero-stability](../../../../../zero-stability.md). A root outside the [unit disk](../../../../../unit-disk.md) causes geometric amplification as $n\sim T/h$ increases; a repeated [unit-circle root](../../../../../unit-circle-root.md) permits polynomial growth in $n$. Either can destroy convergence even for starting perturbations tending to zero.

The [Dahlquist equivalence theorem](../../../../../dahlquist-equivalence-theorem.md) states that, for a fixed-coefficient method and a well-posed [ordinary differential equation](../../../../../ordinary-differential-equation.md) with a suitably [Lipschitz continuous](../../../../../lipschitz-continuity.md) right-hand side, [consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md) and [zero-stability](../../../../../zero-stability.md) are equivalent to convergence for all convergent starting data. If the starting errors are $O(h^p)$ and the exact solution is sufficiently smooth, the global error is $O(h^p)$ on a fixed time interval. A stability estimate bounds the propagated sum of $O(h^{p+1})$ local defects over $O(1/h)$ steps; the [discrete Gronwall inequality](../../../../../discrete-gronwall-inequality.md) controls the dependence of $f$ on the accumulated error. Implicit methods also require the locally consistent, uniquely solvable update branch for sufficiently small $h$.

For example, the [explicit Euler method](../../../../../euler-method.md) has order one and $\rho(\zeta)=\zeta-1$, satisfying the [root condition for a multistep method](../../../../../root-condition-for-a-multistep-method.md). The two-step [Adams-Bashforth method](../../../../../adams-bashforth-method.md) has order two and $\rho(\zeta)=\zeta(\zeta-1)$, again satisfying it. The [trapezoidal rule](../../../../../trapezoidal-rule.md) has order two with one step. The two-step [Simpson multistep method](../../../../../simpson-multistep-method.md), $Y_{n+2}-Y_n=h(f_{n+2}+4f_{n+1}+f_n)/3$, has order four and the simple roots $1,-1$: it is [zero-stable](../../../../../zero-stability.md), although its [parasitic amplification root](../../../../../parasitic-amplification-root.md) can spoil long-time decay. These examples distinguish finite-time [numerical convergence](../../../../../convergence-of-a-numerical-method.md) from [absolute stability](../../../../../linear-stability-domain.md).

The [first Dahlquist barrier](../../../../../first-dahlquist-barrier.md) gives the maximum possible order of a convergent ordinary real $k$-step method:

$$
\boxed{p\le\begin{cases}k+1,&k\text{ odd},\\k+2,&k\text{ even},\end{cases}\qquad p\le k\text{ for an explicit method}.}
$$

These bounds assume only first-derivative evaluations, fixed coefficients and [zero-stability](../../../../../zero-stability.md); the sixth-order [multiderivative multistep method](../../../../../multiderivative-multistep-method.md) in [solution](../5/a/solution.md) is outside that class.

To obtain arbitrarily high convergent order within the ordinary class, increase the number of steps. The [Adams-Bashforth method](../../../../../adams-bashforth-method.md) integrates a [polynomial interpolation](../../../../../polynomial-interpolation.md) of $k$ past derivative values and has order $k$. The [Adams–Moulton method](../../../../../adams-moulton-method.md) includes the new endpoint and has order $k+1$ for $k$ steps. In both families $\rho(\zeta)=\zeta^{k-1}(\zeta-1)$, so the [root condition for a multistep method](../../../../../root-condition-for-a-multistep-method.md) holds for every fixed $k$. Starting values can be generated by a [Runge-Kutta method](../../../../../runge-kutta-method.md) of sufficient accuracy. The [backward differentiation formula](../../../../../backward-differentiation-formula.md) instead differentiates an interpolating [polynomial](../../../../../polynomial-split.md); its order-$k$ members are [zero-stable](../../../../../zero-stability.md) only for $1\le k\le6$.

Finally, high order and favorable stiff stability are separate design goals. By the [Second Dahlquist barrier](../../../../../second-dahlquist-barrier.md), an ordinary [A-stable](../../../../../a-stability.md) [linear multistep method](../../../../../linear-multistep-method.md) has order at most two. One may accept a smaller [linear stability domain](../../../../../linear-stability-domain.md), use suitable [backward differentiation formula](../../../../../backward-differentiation-formula.md) members for stiff problems, or switch to high-order implicit [Runge-Kutta methods](../../../../../runge-kutta-method.md) or [multiderivative multistep methods](../../../../../multiderivative-multistep-method.md). A convergent high-order formula still needs time steps appropriate to its stability properties and the problem's [eigenvalues](../../../../../eigenvalue.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
