<h1 id="b/8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

At a positive interior [maximum](../../../../maximum-of-a-subset-of-a-total-order.md), $u_x=0$, $u_{xx}\leq0$, and $u_t\geq0$ if the point is compared with its past. The PDE instead gives $u_t\leq-u^3<0$, a contradiction. Thus a positive global/past-strip [maximum](../../../../maximum-of-a-subset-of-a-total-order.md) must come from the spatial boundary or initial-time limit. The far value is positive, so any attained global [maximum](../../../../maximum-of-a-subset-of-a-total-order.md) is positive; the argument does not prohibit a negative local [maximum](../../../../maximum-of-a-subset-of-a-total-order.md) in isolation.

For uniqueness put $w=u_1-u_2$. It satisfies

$$
w_t=w_{xx}-\frac{x}{2t}w_x-aw,\qquad a=u_1^2+u_1u_2+u_2^2\geq0.
$$

The [parabolic comparison principle](../../../../parabolic-comparison-principle.md) with zero difference data gives $w\leq0$ and then $-w\leq0$, hence $w=0$. As usual on this noncompact singular-time domain, this uses an admissible comparison class in which the initial and far-field limits justify truncation; for example bounded/subquadratic differences on finite past strips with the corresponding uniform zero traces suffice. A barrier $\delta(1+x^2+2t)$ controls spatial infinity, since $\partial_t-\partial_x^2+[x/(2t)]\partial_x+a$ applied to it is nonnegative. The printed fixed-point limits alone should not silently be substituted for all uniform/growth hypotheses of this comparison argument.

Use [drift cancellation in a parabolic similarity reduction](../../../../drift-cancellation-in-a-parabolic-similarity-reduction.md). For the [similarity ansatz](../../../../similarity-ansatz.md), [derivative](../../../../derivative.md) scaling gives

$$
u_t=t^{-3/2}(-f/2-\beta\eta f'),\quad u_{xx}=t^{-1/2-2\beta}f'',\quad-\frac{x}{2t}u_x=-t^{-3/2}\eta f'/2.
$$

Thus $\boxed{\beta=1/2}$, the drift terms cancel, and $f''=f^3-f/2$ with $f(\infty)=1/\sqrt2$. Use the [positive-equilibrium separatrix for a cubic profile equation](../../../../positive-equilibrium-separatrix-for-a-cubic-profile-equation.md). Multiply by $f'$ and use the limiting [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) to determine the [integration](../../../../integral-split.md) constant:

$$
\frac12(f')^2=\frac14f^4-\frac14f^2+\frac1{16},\qquad(f')^2=\frac12(f^2-1/2)^2.
$$

The branch approaching the positive far [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) satisfies $f'=(1/2-f^2)/\sqrt2$; the constant [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) is included as well. Separation gives

$$
\boxed{f(\eta)=\frac1{\sqrt2}\frac{1-Ae^{-\eta}}{1+Ae^{-\eta}},\qquad
u(x,t)=\frac1{\sqrt{2t}}\frac{1-Ae^{-x/\sqrt t}}{1+Ae^{-x/\sqrt t}}.}
$$

For a finite boundary value at $x=0$ and no interior pole, take $A>-1$. Values $-1<A<0$ describe the corresponding coth-type approach from above; $A=0$ is constant, and positive $A$ gives the tanh-type branch. The other first-integral sign cannot approach the positive [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) nontrivially as $\eta\to\infty$.

The requested deficit integral is, after $x=\sqrt t\eta$,

$$
\int_0^\infty(1/\sqrt{2t}-u)\,dx=\sqrt2\int_0^\infty\frac{Ae^{-\eta}}{1+Ae^{-\eta}}\,d\eta=\sqrt2\log(1+A).
$$

Therefore $\boxed{A=1}$, and the selected solution is $\boxed{u(x,t)=(2t)^{-1/2}\tanh[x/(2\sqrt t)]}$.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the differential equations and applications course of the University of Oxford](../../../split.md)
5. [Differential equations and applications course of the University of Oxford](../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
