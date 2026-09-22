<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [optimization Lagrangian](../../../../../optimization-lagrangian.md) with the sensitivity sign convention

$$
\boxed{L_b(x,\lambda)=f(x)-\lambda^T(h(x)-b),\qquad \lambda\in\mathbb R^m.}
$$

For equality constraints the [Lagrange multipliers](../../../../../lagrange-multiplier.md) have unrestricted signs. The [Lagrangian sufficiency theorem](../../../../../lagrange-sufficiency-theorem.md) says that if $h(x^*)=b$ and, for some $\lambda^*$, $x^*$ globally minimizes $L_b(\cdot,\lambda^*)$ over $X$, then $x^*$ globally minimizes $f$ subject to the constraint. Indeed every feasible $x$ satisfies

$$
f(x)=L_b(x,\lambda^*)\geq L_b(x^*,\lambda^*)=f(x^*).
$$

This proves the theorem without a [convexity](../../../../../convex-function.md) or differentiability assumption. Merely finding a stationary point of the [optimization Lagrangian](../../../../../optimization-lagrangian.md) would not establish its required global minimum.

Let $\phi(u)=\inf\{f(x):x\in X,h(x)=u\}$, with value $+\infty$ when the feasible set is empty, and suppose $\phi(b)$ is finite. The problem has the [Strong Lagrangian property](../../../../../strong-lagrangian-property.md) if a finite multiplier $\lambda$ satisfies

$$
\boxed{\inf_{x\in X}L_b(x,\lambda)=\phi(b).}
$$

This includes attainment of the dual bound by a multiplier. It does not by itself assert attainment of the primal infimum. For every multiplier, restricting the infimum to feasible $x$ gives $\inf_XL_b(x,\lambda)\leq\phi(b)$, the relevant [weak duality](../../../../../weak-duality.md). A [non-vertical supporting hyperplane of a value function](../../../../../non-vertical-supporting-hyperplane-of-a-value-function.md) is a plane

$$
r=\phi(b)+\lambda^T(u-b)
$$

with $\phi(u)\geq\phi(b)+\lambda^T(u-b)$ for every $u$. Its vertical coefficient is nonzero and has been normalized to one; the [epigraph](../../../../../epigraph.md) lies above it. The two directions of the equivalence are proved in parts (a) and (b).

For the sampling allocation put $A=\sum_i\sqrt{a_iv_i}$. Finite [variance](../../../../../variance-split.md) requires every $x_i>0$; interpret the objective at a zero coordinate as $+\infty$. An optimum uses all the budget, because scaling every positive $x_i$ up would otherwise reduce the objective while remaining feasible. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives the global bound

$$
A^2=\left(\sum_i\sqrt{v_i/x_i}\sqrt{a_ix_i}\right)^2\leq\left(\sum_i\frac{v_i}{x_i}\right)\left(\sum_i a_ix_i\right)\leq b\sum_i\frac{v_i}{x_i}.
$$

Equality requires $v_i/x_i$ to be proportional to $a_ix_i$. The budget then determines the unique allocation:

$$
\boxed{x_i^*(b)=\frac bA\sqrt{\frac{v_i}{a_i}},\qquad \phi(b)=\frac{A^2}{b}.}
$$

This is the [optimal cost-constrained stratified sampling allocation](../../../../../optimal-cost-constrained-stratified-sampling-allocation.md).

For an inequality $\sum_i a_ix_i\leq b$, our sign convention uses $\lambda\leq0$, so $L_b=f-\lambda(\sum_i a_ix_i-b)$ is a lower bound on $f$ at feasible points. Its coordinate stationary equations are $-v_i/x_i^2-\lambda a_i=0$, and the displayed allocation gives

$$
\boxed{\lambda^*(b)=-\frac{A^2}{b^2}.}
$$

The function $v_i/x_i+(-\lambda^*)a_ix_i$ has a strict global minimum at $x_i^*$: its second derivative is $2v_i/x_i^3>0$ and its value diverges at both endpoints of $(0,\infty)$. Thus the multiplier also supplies the [Lagrangian sufficiency theorem](../../../../../lagrange-sufficiency-theorem.md) certificate, with the tight inequality giving [complementary slackness](../../../../../complementary-slackness.md).

Finally, for $b+\delta b>0$,

$$
\phi(b+\delta b)-\phi(b)=-\frac{A^2\delta b}{b(b+\delta b)}=\lambda^*(b)\,\delta b+O((\delta b)^2).
$$

Hence **the first-order change in minimal variance is $\boxed{\lambda^*\delta b}$**. Increased resources decrease the variance. With the alternative convention $L=f+\mu(\sum_i a_ix_i-b)$, the multiplier is $\mu=-\lambda^*>0$ and the sensitivity is $-\mu\delta b$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
