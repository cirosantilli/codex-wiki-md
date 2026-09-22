<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the usual [fractional Dirichlet domain scale](../../../../../fractional-dirichlet-domain-scale.md): $A=-\Delta_D$ on $H=L^2(\Omega)$, and $H_\rho=D(A^\rho)$. Its [Sobolev embedding theorem](../../../../../sobolev-embedding-theorem.md) gives

$$
H_\delta\hookrightarrow H^{2\delta}(\Omega)\hookrightarrow C^{0,\beta}(\overline\Omega),\qquad
0<\beta<\min(1,2\delta-n/2).
$$

Such a positive $\beta$ exists precisely because the assumed $\delta$ is greater than $n/4$. Consequently $v=u_t$ is continuous in time with values in this [Hölder space](../../../../../holder-space.md) on every compact positive-time interval. This embedding alone gives no two spatial derivatives for $v$; those must come from the equation.

First establish a bound that will also justify the nonlinear regularity steps. Put $F(s)=\lambda s-s^3$ and

$$
\boxed{K=\max\{|m|,|M|,\sqrt{\max(\lambda,0)}\}.}
$$

The constants $K$ and $-K$ enclose both the initial data and the zero [Dirichlet boundary data](../../../../../dirichlet-boundary-data.md). Moreover $F(K)\leq0$ and $F(-K)\geq0$, so they are a supersolution and a subsolution for the [parabolic comparison principle](../../../../../parabolic-comparison-principle.md). A direct energy proof avoids assuming pointwise continuity at time zero. Let $h=(u-K)_+$. This truncation has zero trace under the [Sobolev trace operator](../../../../../trace-operator.md); testing the evolution with $h$ and using [integration by parts](../../../../../integration-by-parts.md) gives

$$
\frac12\frac d{dt}\|h\|_2^2=-\|\nabla h\|_2^2+\int_\Omega F(u)h\,dx.
$$

For $u>K$, the [mean value theorem](../../../../../mean-value-theorem.md) and $F'(s)=\lambda-3s^2\leq\lambda$ imply $F(u)\leq F(K)+\lambda(u-K)$. Therefore

$$
\frac12\frac d{dt}\|h\|_2^2\leq\lambda\|h\|_2^2.
$$

The [Gronwall inequality](../../../../../gronwall-inequality.md) gives $h=0$, since its initial [L2 norm](../../../../../l2-norm.md) vanishes. For the initially rough datum, apply the inequality from $\varepsilon>0$ and let $\varepsilon\downarrow0$, using $u(\varepsilon)\to u_0$ in [L2 space](../../../../../l2-space-is-a-hilbert-space.md). The same argument for $-u$, which satisfies the same equation because $F$ is odd, proves

$$
\boxed{-K\leq u(x,t)\leq K\quad\text{throughout its existence interval}.}
$$

This is the [invariant interval for a cubic reaction-diffusion equation](../../../../../invariant-interval-for-a-cubic-reaction-diffusion-equation.md); the energy calculation is valid by the [Sobolev chain rule](../../../../../sobolev-chain-rule.md) and approximation even before the stronger pointwise regularity is established.

Now fix $0<\tau<t_0$ and, if necessary, reduce the positive [Hölder exponent](../../../../../holder-exponent.md) $\beta$. Rearranging the evolution gives the elliptic identity

$$
\Delta u(t)=v(t)-F(u(t)),\qquad u(t)|_{\partial\Omega}=0.
$$

Its right side is bounded on $[\tau,t_0]\times\Omega$, because $v\in C([\tau,t_0],C^{0,\beta})$ and $|u|\leq K$. Boundary [elliptic regularity](../../../../../elliptic-regularity.md) first gives $u(t)\in W^{2,p}(\Omega)$ for every finite $p$, uniformly on this time interval. For $p>n$, the [Sobolev embedding theorem](../../../../../sobolev-embedding-theorem.md) makes $u(t)$ spatially continuously differentiable, with a positive [Hölder exponent](../../../../../holder-exponent.md). Thus $F(u(t))$ lies in $C^{0,\beta}$ after reducing $\beta$ if necessary. The [global Schauder estimate](../../../../../global-schauder-estimate.md) then gives $u(t)\in C^{2,\beta}(\overline\Omega)$.

These are continuous-in-time, not just separate-time, regularity statements. Since $v\in C(C^{0,\beta})$, the identity $u(t)-u(s)=\int_s^t v(r)\,dr$, initially an identity in [L2 space](../../../../../l2-space-is-a-hilbert-space.md), holds in $C^{0,\beta}$ once $u(s)$ is known to belong to that space. Hence $u$ is locally Lipschitz in time into $C^{0,\beta}$. Apply the [global Schauder estimate](../../../../../global-schauder-estimate.md) to the difference of the two elliptic identities. Continuity of $v$ and of $F(u)$ into $C^{0,\beta}$ proves $u\in C([\tau,t_0],C^{2,\beta})$.

To gain the spatial regularity of the time derivative itself, take time [difference quotients](../../../../../difference-quotient.md) of the evolution. If $d_h(t)=[u(t+h)-u(t)]/h$, their equations are

$$
(d_h)_t=\Delta d_h+a_h(x,t)d_h,\qquad d_h|_{\partial\Omega}=0,
$$

where

$$
a_h=\lambda-[u(t+h)^2+u(t+h)u(t)+u(t)^2].
$$

The coefficients have uniformly bounded spatial [Hölder norms](../../../../../holder-norm.md) and temporal [Hölder norms](../../../../../holder-norm.md) on compact positive-time cylinders: this follows from the spatial regularity just proved and the local time Lipschitz bound in $C^{0,\beta}$. Also $d_h=\int_0^1v(t+sh)\,ds$ is uniformly bounded and tends to $v$ in $C^{0,\beta}$. Positive-time parabolic [Schauder estimates](../../../../../schauder-estimates.md), applied away from the lower time edge, give uniform $C^{1+\beta/2,2+\beta}$ bounds for $d_h$, with a slightly smaller exponent if needed. Passing to the limit proves that $v$ is continuous into $C^2(\overline\Omega)$ and satisfies

$$
v_t=\Delta v+(\lambda-3u^2)v,\qquad v|_{\partial\Omega}=0.
$$

The [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) for $v$ follows also by differentiating the identically zero boundary value in $C^0$. Since $\tau$ was arbitrary, this proves the requested, genuinely stronger regularity:

$$
\boxed{u\in C^1((0,t_0],C^2(\overline\Omega)).}
$$

This is [positive-time smoothing for a semilinear heat equation](../../../../../positive-time-smoothing-for-a-semilinear-heat-equation.md); it is the extra parabolic step for $v$, not just the [Sobolev embedding theorem](../../../../../sobolev-embedding-theorem.md), that gives the $C^1$ topology asserted here.

Finally, a uniform bound excludes a finite maximal existence time for this [semilinear partial differential equation](../../../../../semilinear-partial-differential-equation.md). Restart at any positive time $s$, using the [heat semigroup](../../../../../heat-semigroup.md) on the [Banach space](../../../../../banach-space-split.md) $X=\{g\in C(\overline\Omega):g|_{\partial\Omega}=0\}$ with the supremum norm. Its [variation-of-constants formula](../../../../../variation-of-constants-formula.md) is

$$
u(s+t)=e^{-tA}u(s)+\int_0^te^{-(t-r)A}F(u(s+r))\,dr.
$$

The [heat semigroup](../../../../../heat-semigroup.md) is a [contraction semigroup](../../../../../contraction-semigroup.md) on $X$. On the ball of radius $K+1$, $F$ is Lipschitz with constant at most $|\lambda|+3(K+1)^2$, and bounded by $|\lambda|(K+1)+(K+1)^3$. Choose a time length $\eta>0$ so that the integral is at most $1$ and its Lipschitz constant is less than $1$. The [Banach fixed-point theorem](../../../../../contraction-mapping-theorem.md) then gives a local solution on $[s,s+\eta]$, with $\eta$ independent of $s$, because $\|u(s)\|_\infty\leq K$. If a finite maximal time existed, choosing $s$ less than $\eta$ before it would extend the same solution past it, a contradiction. Uniqueness identifies this continuation with the original solution, and positive-time smoothing restores the [classical solution](../../../../../classical-solution.md) on each extended interval. **The solution is globally defined and remains between $-K$ and $K$.**

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
