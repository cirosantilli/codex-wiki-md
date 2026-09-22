<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**Available [portfolio wealth](../../../../../portfolio-wealth.md) and the ruin boundary.** Put $h=\bar rD$, the constant interest payment on the fixed loan. The loan principal is already included in available [portfolio wealth](../../../../../portfolio-wealth.md); it is not a growing portfolio holding. Therefore

$$
\boxed{dw=\sigma\theta\,dW+[rw+(\mu-r)\theta-h-c]\,dt,\qquad w_0=x_0+D.}
$$

In particular the interest outflow is $\bar rD$, not $(\bar r-r)D$. Writing $w=x+D$ would instead give net [portfolio wealth](../../../../../portfolio-wealth.md) drift $rx+(\mu-r)\theta-(\bar r-r)D-c$, which explains the distinction.

Let $\tau_0$ denote the ruin time, to avoid confusing it with a fixed terminal horizon. The objective stops at $\tau_0$; consequently **the absorbing boundary is $V(0)=0$**, without an obligation to keep financing the loan after ruin. [Dynamic programming](../../../../../dynamic-programming.md) gives, for $w>0$,

$$
\rho V=(rw-h)V'
+\sup_\theta\{(\mu-r)\theta V'+\tfrac12\sigma^2\theta^2V''\}
+\sup_{c\geq0}\{U(c)-cV'\}.
$$

For increasing strictly [concave](../../../../../concave-function.md) value, put $z=V'(w)>0$ and use [inverse marginal utility](../../../../../inverse-marginal-utility.md) $I$. The optimal controls and the optimized [HJB equation](../../../../../hamilton-jacobi-bellman-equation.md) are

$$
c^*=I(z),\qquad \theta^*=-\frac{\kappa}{\sigma}\frac{V'}{V''},\qquad
0=(rw-h)V'-\rho V-\frac{\kappa^2(V')^2}{2V''}+\widetilde U(V'),
$$

where $\widetilde U(z)=\sup_{c\geq0}[U(c)-zc]$. For [CRRA utility](../../../../../constant-relative-risk-aversion-utility.md) with $0<R<1$, write $p=1-R$ and $q=1-1/R<0$. Then

$$
I(z)=z^{-1/R},\qquad \widetilde U(z)=\frac R p z^q.
$$

**Dualization and the printed constant.** Use the convex [wealth-variable Legendre dual](../../../../../wealth-variable-legendre-dual.md)

$$
J(z)=\sup_{w\geq0}[V(w)-zw].
$$

At an interior maximizing [portfolio wealth](../../../../../portfolio-wealth.md), $J'=-w$, $J''=-1/V''>0$ and $V=J-zJ'$. The dual [HJB equation](../../../../../hamilton-jacobi-bellman-equation.md) is the linear [Euler differential equation](../../../../../cauchy-euler-equation.md)

$$
\boxed{\tfrac12\kappa^2z^2J''+(\rho-r)zJ'-\rho J-hz+\frac R p z^q=0.}
$$

A trial power $z^t$ gives

$$
Q(t)=\tfrac12\kappa^2t(t-1)+(\rho-r)t-\rho.
$$

Direct substitution gives

$$
Q(q)=-\gamma_M,\qquad
\boxed{\gamma_M=\frac{\rho+(R-1)(r+\kappa^2/(2R))}{R}.}
$$

The PDF prints an additional factor $1/2$ before $\kappa^2/(2R)$ in its definition of $\gamma_M$. That printed definition is inconsistent with its own identity for $Q(q)$. The expression above is the one used here; assume this corrected $\gamma_M>0$.

**Solution when $\kappa\ne0$.** Assume positive discount $\rho$, nonzero $\sigma$, and $h>0$. Let $m>0$ and $n<0$ be the two roots of $Q$:

$$
m,n=\frac{-(\rho-r-\kappa^2/2)\ \pm\
\sqrt{(\rho-r-\kappa^2/2)^2+2\kappa^2\rho}}{\kappa^2}.
$$

Since $Q(q)<0$, $n<q<0<m$. Put $C=R/(p\gamma_M)$. For $r\ne0$, the general interior solution is

$$
J(z)=Az^m+Bz^n-\frac h r z+Cz^q.
$$

The appropriate large-wealth condition is the [Merton consumption-investment problem](../../../../../merton-consumption-investment-problem.md) bound

$$
0\leq V(w)\leq \frac{\gamma_M^{-R}}p\,w^p.
$$

Indeed any original control consumes $c+h$ in the debt-free comparison model until ruin, and $U(c+h)\geq U(c)$. Dualizing this bound gives $0\leq J(z)\leq Cz^q$. Because $n<q$, convexity and this upper bound force **$B=0$** as $z\downarrow0$.

At the other endpoint [portfolio wealth](../../../../../portfolio-wealth.md) reaches zero. If $z_*=V'(0+)$, the [dual ruin boundary with debt service](../../../../../dual-ruin-boundary-with-debt-service.md) requires

$$
\boxed{J(z_*)=0,\qquad J'(z_*)=0,\qquad J(z)=0\quad(z\geq z_*).}
$$

Solving these two equations gives

$$
\boxed{
z_*=\left[\frac{Cr(m-q)}{h(m-1)}\right]^R,\qquad
A=\frac{C(1-q)}{m-1}\,z_*^{q-m}.}
$$

For $r>0$, $m>1$, and for $r<0$, $0<m<1$, so the quantity defining $z_*$ is positive in either case. These formulas determine the entire value. For each $w>0$, choose the unique $z\in(0,z_*)$ satisfying

$$
\boxed{w=\frac h r-Amz^{m-1}-Cqz^{q-1}.}
$$

Then

$$
\boxed{V(w)=A(1-m)z^m+C(1-q)z^q,\qquad
c^*=z^{-1/R},\qquad
\theta^*=\frac{\kappa z}{\sigma}
\left[Am(m-1)z^{m-2}+Cq(q-1)z^{q-2}\right].}
$$

Both terms in the bracket are positive, even when $r<0$ and $A<0$. Thus $J''>0$, $-J'$ decreases from infinity to zero as $z$ increases, and the [portfolio wealth](../../../../../portfolio-wealth.md) inversion really is unique. The extended dual is continuously differentiable and convex.

There is no additional condition $J''(z_*^-)=0$. In fact

$$
J''(z_*^-)=C(1-q)(m-q)z_*^{q-2}>0.
$$

Available [portfolio wealth](../../../../../portfolio-wealth.md) is killed at zero; the portfolio can have a nonzero limiting volatility immediately before ruin. Imposing a reflecting-boundary or zero-curvature condition would solve a different problem.

For $r=0$, the linear forcing resonates with the root $m=1$. Put $b=\rho+\kappa^2/2=Q'(1)$. The dual and boundary constants instead are

$$
\boxed{\begin{aligned}
J(z)&=Az+\frac h b z\log z+Cz^q &&(0<z<z_*),\\
z_*&=\left[\frac{Cb(1-q)}h\right]^R,\qquad
A=-\frac h b\log z_*-Cz_*^{q-1}.
\end{aligned}}
$$

Extend by zero for $z\geq z_*$. Here

$$
w=-A-\frac h b(\log z+1)-Cqz^{q-1},\qquad
V(w)=C(1-q)z^q-\frac h b z,
$$

and the controls remain $c=z^{-1/R}$ and $\theta=\kappa zJ''/\sigma$, with $J''=h/(bz)+Cq(q-1)z^{q-2}>0$.

**Verification and transversality.** The candidate is nonnegative, increasing, strictly [concave](../../../../../concave-function.md) and zero at ruin. Its [HJB equation](../../../../../hamilton-jacobi-bellman-equation.md) makes the discounted value plus accrued utility a [local supermartingale](../../../../../local-supermartingale.md) for every admissible control, and a [local martingale](../../../../../local-martingale.md) for the stated feedback. Localization at positive lower and finite upper [portfolio wealth](../../../../../portfolio-wealth.md) levels gives the finite-horizon comparison. The [investment value transversality condition](../../../../../investment-value-transversality-condition.md) follows from the same debt-free bound: applying the [Itô formula](../../../../../ito-s-lemma.md) to $w^p$ and maximizing its risky term gives

$$
\mathbb E[e^{-\rho t}w_t^p\mathbf1_{\{t<\tau_0\}}]
\leq w_0^p e^{-[\rho-p(r+\kappa^2/(2R))]t}
=w_0^p e^{-R\gamma_M t}.
$$

The nonnegative [consumption](../../../../../consumption.md) and debt-service drifts only decrease this bound. Thus the expected terminal candidate tends to zero. The feedback has at most linear growth, including a finite limit as [portfolio wealth](../../../../../portfolio-wealth.md) decreases to zero; stopping it at ruin gives an admissible policy. Letting localization levels and then the horizon tend to their limits proves that the candidate is the value, rather than just a formal dual solution. If $D=0$, the absorbing-debt boundary disappears and the ordinary [Merton consumption-investment problem](../../../../../merton-consumption-investment-problem.md) formula is recovered.

**Zero market price of risk.** With $\sigma\ne0$ and $\kappa=0$, the dual equation is first order. If $\rho>r$, the preceding formulas remain valid with $m=\rho/(\rho-r)$ for $r\ne0$, and the logarithmic formula with $b=\rho$ for $r=0$; there is no $B$ term and $\theta^*=0$. The same boundary and transversality argument verifies this deterministic [consumption](../../../../../consumption.md) policy.

The remaining finite-value case has $r>0$ and $pr<\rho\leq r$. Put $\gamma_0=(\rho-pr)/R$, $w_c=h/(rR)$ and

$$
z_c=\left(\frac{Rr}{p\gamma_0h}\right)^R.
$$

The correct convex dual and its corresponding value are

$$
\boxed{
J(z)=\max\left\{\frac{R}{p\gamma_0}z^q-\frac h r z,\ 0\right\},\qquad
V(w)=
\begin{cases}
z_cw,&0\leq w\leq w_c,\\
\gamma_0^{-R}(w-h/r)^p/p,&w\geq w_c.
\end{cases}}
$$

The two value branches have the same value and derivative at $w_c$. Above $w_c$, hold no stock and consume $\gamma_0(w-h/r)$; the surplus over $h/r$ grows at rate $r-\gamma_0\geq0$. If $\rho=r$, the lower branch is attained by zero stock holding and constant [consumption](../../../../../consumption.md) $ph/R$: [portfolio wealth](../../../../../portfolio-wealth.md) solves $\dot w=r(w-w_c)$ until ruin, and direct integration gives $z_cw$.

If $\rho<r$ and $0<w<w_c$, the lower branch is a supremum attained in a limit of increasingly rapid fair stock lotteries between zero and $w_c$, followed by the upper-branch policy on success. The success probability tends to $w/w_c$ and the fixed service cost during the lottery tends to zero. This is possible because unrestricted dollar holdings in the nonzero-volatility stock produce a fair [Brownian motion](../../../../../brownian-motion-split.md) exposure even when its excess drift is zero. The supporting linear branch has optimized waiting residual $(r-\rho)z_c(w-w_c)<0$; the fast lotteries, rather than a finite feedback optimizer, supply the missing control limit. The piecewise candidate is [concave](../../../../../concave-function.md), has nonpositive waiting residual everywhere, and the preceding moment bound still supplies an upper-bound verification. **This degenerate case can have a supremum without an ordinary maximizing strategy.**

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
