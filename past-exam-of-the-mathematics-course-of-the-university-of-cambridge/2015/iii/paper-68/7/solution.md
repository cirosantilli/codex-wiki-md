<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Consider an [initial value problem](../../../../../initial-value-problem.md) $y'=f(t,y)$ on $[0,T]$, with a [Lipschitz continuous](../../../../../lipschitz-continuity.md) [vector field](../../../../../vector-field.md) in the solution variable and enough smoothness for the stated error expansions. [Convergence of a numerical method](../../../../../convergence-of-a-numerical-method.md) means

$$
 \max_{t_n\leq T}\|Y_n-y(t_n)\|\longrightarrow0\qquad(h\to0),
$$

with consistent starting values. An [order of a numerical method](../../../../../order-of-a-numerical-method.md) $p$ quantifies this approximation: with sufficiently accurate starting data and the required stability, the [global error](../../../../../global-discretization-error.md) is $O(h^p)$. [Stability of a numerical method](../../../../../stability-of-a-numerical-method.md) controls the amplification and accumulation of perturbations; it is the link between a small local defect and small global error.

For a one-step formula $Y_{n+1}=\Phi_h(t_n,Y_n)$, define the unscaled [local truncation error](../../../../../local-truncation-error.md)

$$
 d_{n+1}=y(t_{n+1})-\Phi_h(t_n,y(t_n)).
$$

The method has local order $p$ if $\|d_{n+1}\|\leq Ch^{p+1}$ uniformly along sufficiently smooth solutions. If the defect is divided by $h$, its order is instead $O(h^p)$; the convention must be specified. Assume also the perturbation estimate

$$
 \|\Phi_h(t,u)-\Phi_h(t,v)\|\leq(1+L_\Phi h)\|u-v\|.
$$

The [global error](../../../../../global-discretization-error.md) $e_n=Y_n-y(t_n)$ then satisfies

$$
 \|e_{n+1}\|\leq(1+L_\Phi h)\|e_n\|+Ch^{p+1}.
$$

Iterating, or applying the [discrete Gronwall inequality](../../../../../discrete-gronwall-inequality.md), gives

$$
\boxed{\max_{nh\leq T}\|e_n\|\leq e^{L_\Phi T}\bigl(\|e_0\|+CT h^p\bigr).}
$$

There are $O(1/h)$ steps on a fixed interval, so stable propagation turns $O(h^{p+1})$ local defects into $O(h^p)$ accumulated error. Starting error $O(h^p)$ is needed to retain order $p$. This explains why matching an exact [Taylor expansion](../../../../../taylor-expansion.md) is insufficient unless errors are controlled during repeated steps.

For a fixed-coefficient [linear multistep method](../../../../../linear-multistep-method.md), write

$$
 \sum_{j=0}^s\alpha_jY_{n+j}=h\sum_{j=0}^s\beta_jf(t_{n+j},Y_{n+j}),\quad
 \rho(\zeta)=\sum_j\alpha_j\zeta^j,\quad
 \sigma(\zeta)=\sum_j\beta_j\zeta^j.
$$

The [consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md) conditions are $\rho(1)=0$ and $\rho'(1)=\sigma(1)$. The higher [order conditions for a linear multistep method](../../../../../order-conditions-for-a-linear-multistep-method.md) are

$$
 \sum_j\alpha_jj^q=q\sum_j\beta_jj^{q-1},\qquad q=0,\ldots,p,
$$

with right side zero for $q=0$; exact order $p$ means first failure at $q=p+1$. They come from inserting the exact solution and comparing its [Taylor expansion](../../../../../taylor-expansion.md).

Errors at $h=0$ follow the homogeneous recurrence determined by $\rho$. [Zero-stability](../../../../../zero-stability.md) is equivalent to the [root condition for a multistep method](../../../../../root-condition-for-a-multistep-method.md): all [roots of a polynomial](../../../../../root-of-a-polynomial.md) have [modulus](../../../../../modulus.md) at most one, and every unit-modulus root is simple. Roots outside the disk give exponential growth in the number of steps; repeated unit roots give polynomial growth in that number. Repeated interior roots are harmless because their polynomial factors are dominated by decay. Under the usual [Lipschitz continuity](../../../../../lipschitz-continuity.md) and initialization assumptions, the [Dahlquist equivalence theorem](../../../../../dahlquist-equivalence-theorem.md) gives

$$
\boxed{\text{convergence}=\text{consistency plus zero-stability}.}
$$

For a zero-stable order-$p$ [linear multistep method](../../../../../linear-multistep-method.md), local defects and starting errors of the stated orders yield [global error](../../../../../global-discretization-error.md) $O(h^p)$ by a recurrence bound and the [discrete Gronwall inequality](../../../../../discrete-gronwall-inequality.md). Every required starting value matters.

A concrete failure of “consistency implies convergence” is

$$
 Y_{n+2}-3Y_{n+1}+2Y_n=-h f(t_n,Y_n).
$$

Here $\rho=(\zeta-1)(\zeta-2)$ and $\sigma=-1$, so $\rho(1)=0$ and $\rho'(1)=\sigma(1)=-1$: the method is consistent, of order one. But its root $2$ violates [zero-stability](../../../../../zero-stability.md). For $y'=0$ with exact solution zero and starting values $Y_0=0$, $Y_1=h^2$, the computed solution is $Y_n=h^2(2^n-1)$. These starting errors vanish, yet at $n\approx T/h$ the error diverges. Local accuracy cannot compensate for an unstable recurrence.

A different meaning of [stability](../../../../../stability-of-a-numerical-method.md) concerns a fixed step on decaying equations. The [Dahlquist test equation](../../../../../dahlquist-test-equation.md) $y'=\lambda y$ introduces $z=h\lambda$. A one-step method gives $Y_{n+1}=R(z)Y_n$ and is absolutely stable when $|R(z)|\leq1$. For a [linear multistep method](../../../../../linear-multistep-method.md), the corresponding [amplification polynomial of a multistep method](../../../../../amplification-polynomial-of-a-multistep-method.md) is $\rho(\zeta)-z\sigma(\zeta)$, and every root must satisfy the bounded root condition, not just the root approximating $e^z$. Strict asymptotic decay requires the roots to have [modulus](../../../../../modulus.md) less than one for $\operatorname{Re}z<0$. This distinction matters at reducible methods with an undamped parasitic mode, as in question 1(c).

The [Forward Euler method](../../../../../euler-method.md) has order one and $R(z)=1+z$, so its [linear stability domain](../../../../../linear-stability-domain.md) is $|1+z|\leq1$. For $y'=-\kappa y$, with $\kappa>0$, it requires $0\leq h\kappa\leq2$. It converges as $h\to0$, yet an excessively large step can produce growing oscillations on an exactly decaying problem. The [Backward Euler method](../../../../../backward-euler-method.md) has the same order, but $R(z)=(1-z)^{-1}$ makes it [A-stable](../../../../../a-stability.md) and [L-stable](../../../../../l-stability.md). For a [stiff differential equation](../../../../../stiff-equation.md), fast decay can impose a severe explicit time-step restriction even when accuracy of the slow dynamics would permit a much larger step.

The [trapezoidal rule](../../../../../trapezoidal-rule.md) has order two and is [A-stable](../../../../../a-stability.md), but is not [L-stable](../../../../../l-stability.md), since its [stability function](../../../../../stability-function.md) tends to $-1$ along the negative real axis. The [Second Dahlquist barrier](../../../../../second-dahlquist-barrier.md) limits an irreducible [A-stable](../../../../../a-stability.md) [linear multistep method](../../../../../linear-multistep-method.md) to order at most two. This does not limit implicit [Runge-Kutta methods](../../../../../runge-kutta-method.md): question 4's [Lobatto IIIA method](../../../../../lobatto-iiia-method.md) is fourth-order and [A-stable](../../../../../a-stability.md). Conversely, question 1's fourth-order member is convergent but not [A-stable](../../../../../a-stability.md). These examples show that [order of a numerical method](../../../../../order-of-a-numerical-method.md), [zero-stability](../../../../../zero-stability.md) and [A-stability](../../../../../a-stability.md) answer different questions.

For nonlinear dissipative problems, [B-stability](../../../../../b-stability.md) controls distances between numerical solutions; [algebraic stability of a Runge-Kutta method](../../../../../algebraic-stability-of-a-runge-kutta-method.md) is a sufficient coefficient criterion. Question 4 shows that [A-stability](../../../../../a-stability.md) alone does not imply that coefficient criterion. Variable time steps require additional analysis of step ratios and error propagation, and stiff problems may require uniform-in-stiffness error estimates beyond the fixed-problem convergence result. **The useful chain is local accuracy plus the appropriate perturbation bound, giving global accuracy; absolute and nonlinear stability then determine which practical time steps preserve the intended dynamics.**

## ↑ Ancestors (11)

1. [7](../7.md)
2. [Section B](../section-b.md)
3. [Paper 68](../../paper-68-split.md)
4. [Iii](../../split.md)
5. [2015](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
