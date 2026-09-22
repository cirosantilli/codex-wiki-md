<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

For an [initial value problem](../../../../../initial-value-problem.md), [convergence of a numerical method](../../../../../convergence-of-a-numerical-method.md) means that on each fixed interval $0\le t\le T$, the largest error at mesh points tends to zero as the step size tends to zero and the starting errors vanish. [Order of a numerical method](../../../../../order-of-a-numerical-method.md) describes how rapidly an exact-start local defect decreases; [stability of a numerical method](../../../../../stability-of-a-numerical-method.md) controls propagation of that defect and of errors already present. These are related but different properties. A high-order expansion alone cannot ensure that accumulated error remains small.

For a one-step map $Y_{n+1}=\Phi_h(t_n,Y_n)$, define the exact-start defect $d_{n+1}=y(t_{n+1})-\Phi_h(t_n,y(t_n))$. Order $p$ means $d_{n+1}=O(h^{p+1})$ for sufficiently smooth solutions. The normalized [local truncation error](../../../../../local-truncation-error.md) divides this defect by $h$ and is $O(h^p)$; explicitly specifying the normalization prevents an apparent one-order discrepancy. Suppose the map satisfies the local Lipschitz bound

$$
\|\Phi_h(t,u)-\Phi_h(t,v)\|\le(1+Lh)\|u-v\|.
$$

For $e_n=Y_n-y(t_n)$ the error recurrence is

$$
\|e_{n+1}\|\le(1+Lh)\|e_n\|+Ch^{p+1}.
$$

Iteration, or the [discrete Gronwall inequality](../../../../../discrete-gronwall-inequality.md), yields $\|e_n\|\le e^{LT}(\|e_0\|+CT h^p)$ for $nh\le T$. **Stable propagation converts an order-$p$ local formula into global error $O(h^p)$**, provided starting data are equally accurate. Consistency is the weaker requirement that the normalized local defect tend to zero.

For a [linear multistep method](../../../../../linear-multistep-method.md), [zero-stability](../../../../../zero-stability.md) concerns the recurrence at $h=0$. Its roots must have modulus at most one, and unit-modulus roots must be simple. Roots outside the circle amplify errors exponentially in the number of steps; repeated unit roots introduce polynomial growth. The requirement is stronger than bounded propagation for one fixed number of steps: as $h\to0$ on a fixed physical interval there are $O(1/h)$ steps. Under the usual Lipschitz assumptions and consistent starting values, the [Dahlquist equivalence theorem](../../../../../dahlquist-equivalence-theorem.md) says consistency plus zero-stability is equivalent to convergence. Its sufficiency combines a bounded discrete recurrence propagator with the sum of local defects, while necessity follows by exciting an unstable homogeneous root or by observing the persistent error of an inconsistent formula.

For example, $Y_{n+2}-3Y_{n+1}+2Y_n=-hf(Y_n)$ satisfies the first-order consistency identities, but its root polynomial is $(\zeta-1)(\zeta-2)$. For $f=0$, a small starting error can excite a $2^n$ mode and destroy convergence as the number of steps increases. In contrast, simple parasitic unit roots such as the root minus one of a two-step centered method need not destroy zero-stability: they remain bounded, though they can create unwanted oscillations and affect practical behavior. Accurate starting procedures and suppression of accumulated parasitic error remain relevant.

[Absolute stability](../../../../../linear-stability-domain.md) asks a different question: for $y'=\lambda y$, does the discrete solution decay or stay bounded for a specified finite $z=h\lambda$? The [Forward Euler method](../../../../../euler-method.md) has $R(z)=1+z$ and, for real $\lambda<0$, requires $h\le2/|\lambda|$. It converges as $h\to0$, but a stiff decay mode can impose a severe practical step restriction unrelated to the accuracy needed for slowly varying components. The [Backward Euler method](../../../../../backward-euler-method.md) has $R(z)=1/(1-z)$, hence is [A-stable](../../../../../a-stability.md) and [L-stable](../../../../../l-stability.md). The [trapezoidal rule](../../../../../trapezoidal-rule.md) has $R(z)=(1+z/2)/(1-z/2)$, is A-stable, but tends to minus one on a very stiff negative mode and can retain alternating transients rather than damping them rapidly.

Zero-stability therefore does not imply unrestricted absolute stability; the three-step family analyzed earlier in this paper is a particularly strong illustration. Conversely a stable large step need not be accurate. This distinction matters for a [stiff equation](../../../../../stiff-equation.md). The [Second Dahlquist barrier](../../../../../second-dahlquist-barrier.md) limits A-stable linear multistep methods to order at most two, whereas implicit [Runge-Kutta methods](../../../../../runge-kutta-method.md) can have much higher order and still be A-stable. That barrier concerns the specified method class, not every numerical time integrator.

Finally, the mathematical order depends on smoothness: nonsmooth solutions or forcing can lower observed rates. Roundoff, imperfect implicit solves and inaccurate derivative evaluations introduce additional defects. Smaller steps increase the number of such perturbations; truncation error alone does not describe arbitrarily fine computation. The useful organizing principle is **consistency supplies vanishing defects, stability bounds their accumulation, convergence follows, and order quantifies its rate under the stated regularity and starting-error assumptions**.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
