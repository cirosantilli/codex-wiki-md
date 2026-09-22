# Paper 40

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_40.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_40.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

**Wealth and admissibility.** The dollar holding $\theta$ earns the risky return, while $w-\theta$ earns the [continuous-time bank account](../../../mathematical-finance.md#continuous-time-bank-account) return. Removing [consumption](../../../mathematical-finance.md#consumption) therefore gives

$$
\boxed{dw_t=\sigma\theta_t\,dW_t+\bigl[rw_t+(\mu-r)\theta_t-c_t\bigr]dt.}
$$

Here $\theta$ is a dollar amount, not a number of shares; the number of shares is $\theta_t/S_t$. Both controls must use available information: take $\theta$ [predictable](../../../martingale.md#predictable-process) and $c\geq0$ [progressively measurable](../../../stochastic-process.md#progressive-measurability), with

$$
\int_0^t(\sigma\theta_s)^2ds<\infty,\qquad
\int_0^t\bigl(|(\mu-r)\theta_s|+c_s\bigr)ds<\infty
$$

almost surely on every finite interval. Require a well-defined objective and an [admissible trading strategy](../../../mathematical-finance.md#admissible-trading-strategy) satisfying $w_t\geq0$. At zero [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) this excludes continued risky gambling or positive [consumption](../../../mathematical-finance.md#consumption). The [state-price budget constraint](../../../mathematical-finance.md#state-price-budget-constraint) rules out doubling strategies. Throughout the diffusion calculations take $\sigma\ne0$, positive discount $\rho$, positive decay $\lambda$, and finite value; degeneracies are discussed where they affect the conclusions.

**Satisfaction and dynamic programming.** Write the [consumption satisfaction stock](../../../utility-function.md#consumption-satisfaction-stock) as

$$
\xi_t=e^{-\lambda t}\left(\xi_0+\int_0^t e^{\lambda s}c_sds\right).
$$

The [product rule](../../../calculus.md#product-rule) gives, almost everywhere in time,

$$
\boxed{d\xi_t=(c_t-\lambda\xi_t)\,dt.}
$$

This state is a [finite-variation process](../../../stochastic-calculus.md#finite-variation-process), so it has no [quadratic covariation](../../../stochastic-calculus.md#quadratic-covariation) with [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth). Applying the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to the discounted [value function](../../../mathematical-optimization.md#value-function) over a short interval, then using [dynamic programming](../../../mathematical-optimization.md#dynamic-programming), gives the interior [HJB equation](../../../mathematical-optimization.md#hamilton-jacobi-bellman-equation)

$$
0=U(\xi)-\rho V+rwV_w-\lambda\xi V_\xi
+\sup_{\theta\in\mathbb R}\left\{(\mu-r)\theta V_w+\frac{\sigma^2\theta^2}{2}V_{ww}\right\}
+\sup_{c\geq0}c(V_\xi-V_w).
$$

Assuming $V_{ww}<0$, completing the square gives

$$
\theta^*=-\frac{\mu-r}{\sigma^2}\frac{V_w}{V_{ww}},
\qquad
\sup_\theta\{\cdots\}=-\frac{\kappa^2}{2}\frac{V_w^2}{V_{ww}},
\qquad
\kappa=\frac{\mu-r}{\sigma}.
$$

The last supremum is zero if $V_\xi-V_w\leq0$ and infinite otherwise. Thus **the [gradient constraint for unbounded consumption](../../../utility-function.md#gradient-constraint-for-unbounded-consumption) is $V_\xi\leq V_w$, and $c=0$ wherever the inequality is strict.** Since there is no direct penalty for a very large [consumption](../../../mathematical-finance.md#consumption) rate, an active boundary can involve [singular consumption control](../../../utility-function.md#singular-consumption-control). In that relaxed interpretation the [HJB equation](../../../mathematical-optimization.md#hamilton-jacobi-bellman-equation) is

$$
\max\left\{U(\xi)-\rho V+rwV_w-\lambda\xi V_\xi
-\frac{\kappa^2}{2}\frac{V_w^2}{V_{ww}},\ V_\xi-V_w\right\}=0.
$$

With ordinary rate controls, this describes the supremum and its limiting transfer policy; it does not promise that an instantaneous transfer is attained by a finite rate.

**Power reduction.** An additive constant in the [utility function](../../../utility-function.md) only adds a control-independent constant divided by $\rho$ to the value, so normalize $U(\xi)=\xi^{1-R}/(1-R)$. Put $p=1-R$ and $x=w/\xi$ for $\xi>0$. Scaling [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth), [consumption satisfaction](../../../utility-function.md#consumption-satisfaction-stock) and the controls by the same positive number gives the [wealth-to-satisfaction reduction](../../../utility-function.md#wealth-to-satisfaction-reduction)

$$
V(\xi,w)=\xi^p v(x),\qquad
V_w=\xi^{-R}v',\quad
V_{ww}=\xi^{-R-1}v'',\quad
V_\xi=\xi^{-R}(pv-xv').
$$

Consequently the reduced [HJB equation](../../../mathematical-optimization.md#hamilton-jacobi-bellman-equation) is

$$
\boxed{\max\left\{
\frac1p-[\rho+\lambda p]v+(r+\lambda)xv'
-\frac{\kappa^2}{2}\frac{(v')^2}{v''},
\ pv-(x+1)v'
\right\}=0.}
$$

In the strict waiting region the first expression vanishes and [consumption](../../../mathematical-finance.md#consumption) is zero. On a transfer region the second vanishes; integrating it gives $v(x)=K(1+x)^p$. This reflects preservation of $w+\xi$ during an instantaneous wealth-to-satisfaction transfer.

**Why a waiting threshold is expected, and its qualification.** The [gradient constraint for unbounded consumption](../../../utility-function.md#gradient-constraint-for-unbounded-consumption) compares the benefit of increasing [consumption satisfaction](../../../utility-function.md#consumption-satisfaction-stock) with the opportunity cost of spending financial [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth). When [consumption satisfaction](../../../utility-function.md#consumption-satisfaction-stock) is already large relative to cash, waiting lets [consumption satisfaction](../../../utility-function.md#consumption-satisfaction-stock) decay while financial [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) earns returns; consuming immediately can be wasteful. [Homogeneity](../../../real-analysis.md#homogeneity) makes the comparison depend only on $x$. For fixed $s=w+\xi$, joint [concavity](../../../real-analysis.md#concave-function) of the [value function](../../../mathematical-optimization.md#value-function) makes $q_s(a)=V(s-a,a)$ [concave](../../../real-analysis.md#concave-function) in financial [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) $a$. It is nondecreasing because an immediate transfer can reproduce any smaller financial allocation. Consequently its derivative $V_w-V_\xi$ is nonnegative and nonincreasing in $a$: a strict waiting region, if present, starts at zero financial [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) and ends at a single transfer boundary. [Homogeneity](../../../real-analysis.md#homogeneity) makes the corresponding boundary a ratio $x_*$. In the usual finite-boundary regime this gives $c=0$ for $x<x_*$, and transfers push a larger ratio down towards $x_*$. The condition is a comparison of marginal values, not the ordinary formula $c=(V_w)^{-1/R}$: current [utility function](../../../utility-function.md) here depends on [consumption satisfaction](../../../utility-function.md#consumption-satisfaction-stock), not on current [consumption](../../../mathematical-finance.md#consumption).

A positive threshold is not guaranteed by the printed hypotheses alone. A useful sufficient local test illustrates the intended argument. Let $a=\rho+\lambda p>0$. At zero [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth),

$$
V(\xi,0)=\frac{\xi^p}{pa},\qquad V_\xi(\xi,0)=\frac{\xi^{-R}}a.
$$

Starting with a small extra [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) $\varepsilon$, holding it in the [continuous-time bank account](../../../mathematical-finance.md#continuous-time-bank-account) until a fixed time $t$, then transferring it into [consumption satisfaction](../../../utility-function.md#consumption-satisfaction-stock), has right derivative in $\varepsilon$ at zero equal to

$$
\frac{\xi^{-R}}a\,e^{(r-\rho+\lambda R)t}.
$$

Therefore, if $\rho<r+\lambda R$, the [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) marginal value is strictly larger than the [consumption satisfaction](../../../utility-function.md#consumption-satisfaction-stock) marginal value at zero. With the usual continuity of marginal values, there is a positive interval on which the [gradient constraint for unbounded consumption](../../../utility-function.md#gradient-constraint-for-unbounded-consumption) is strict. The fixed-total-resource [concavity](../../../real-analysis.md#concave-function) argument then gives the threshold structure.

For a concrete counterexample to an unconditional positive threshold, take $R=1/2$, $\lambda=1$, $r=\mu=1/10$, $\sigma=1$ and $\rho=2$. There is zero [market price of risk](../../../mathematical-finance.md#market-price-of-risk). The relaxed value is

$$
F(\xi,w)=\frac{(\xi+w)^p}{pa},\qquad p=\frac12,\quad a=\frac52.
$$

Indeed $F_\xi=F_w$, $F_{ww}<0$, and the optimized waiting residual, after division by $\xi^p$, is

$$
-\int_0^x(1+s)^{-R}ds+\frac{r+\lambda}{a}x(1+x)^{-R}\leq0,
$$

because $(r+\lambda)/a<1$ and the integrand is decreasing. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives an upper bound by $F$, while transferring all [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) into [consumption satisfaction](../../../utility-function.md#consumption-satisfaction-stock) over intervals tending to zero attains that bound in the limit. Hence the transfer boundary is $x_*=0$ in this example. **The positive-threshold explanation needs a parameter regime supporting a genuine waiting region.** For $R>1$, even the zero-wealth value is finite only if $\rho>\lambda(R-1)$; otherwise decaying [consumption satisfaction](../../../utility-function.md#consumption-satisfaction-stock) gives value $-\infty$.

## 2

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

**The joint generator.** With $\theta$ again measured in dollars, [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) obeys

$$
dw=\sigma(x)\theta\,dW+[rw+(\mu(x)-r)\theta-c]\,dt.
$$

Its noise and the factor noise are driven by the same [Brownian motion](../../../brownian-motion.md). Their [quadratic covariation](../../../stochastic-calculus.md#quadratic-covariation) is $\sigma(x)\theta\alpha(x)\,dt$, so the [diffusion generator](../../../stochastic-process.md#diffusion-generator) has a cross derivative. [Dynamic programming](../../../mathematical-optimization.md#dynamic-programming) and the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) give

$$
\boxed{\begin{aligned}
0={}&\tfrac12\alpha^2V_{xx}+\beta V_x-\rho V+rwV_w\\
&+\sup_{\theta\in\mathbb R}
\left\{(\mu-r)\theta V_w+\sigma\alpha\theta V_{wx}
+\tfrac12\sigma^2\theta^2V_{ww}\right\}
+\sup_{c\geq0}\{U(c)-cV_w\}.
\end{aligned}}
$$

All coefficient functions in this formula are evaluated at $x$. The cross derivative is essential: it gives [intertemporal hedging demand](../../../utility-function.md#intertemporal-hedging-demand). Normalizing [CRRA utility](../../../utility-function.md#constant-relative-risk-aversion-utility) as $U(c)=c^p/p$, where $p=1-R$, the two optimizations give, at nonzero volatility,

$$
c^*=(V_w)^{-1/R},\qquad
\theta^*=-\frac{(\mu-r)V_w+\sigma\alpha V_{wx}}{\sigma^2V_{ww}},
$$

and hence

$$
0=\tfrac12\alpha^2V_{xx}+\beta V_x-\rho V+rwV_w
-\frac{[(\mu-r)V_w+\sigma\alpha V_{wx}]^2}{2\sigma^2V_{ww}}
+\frac R p(V_w)^{p(-1/R)}.
$$

Here $p(-1/R)=1-1/R$.

**Homogeneity and the reduced equation.** Scaling initial [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) and both controls preserves the [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) constraint and multiplies the objective by the positive number $b^p$. Thus

$$
V(w,x)=\frac{w^p}{p}f(x),\qquad f(x)>0.
$$

This expression is valid for both signs of $p$: $V$ is negative when $R>1$, but its [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) derivative is positive. Its derivatives are

$$
V_w=w^{-R}f,\quad V_{ww}=-Rw^{-R-1}f,\quad
V_{wx}=w^{-R}f',\quad
V_x=\frac{w^p}{p}f',\quad V_{xx}=\frac{w^p}{p}f''.
$$

Substitution yields

$$
\boxed{
\tfrac12\alpha^2f''+\beta f'+(pr-\rho)f
+\frac{p[(\mu-r)f+\sigma\alpha f']^2}{2R\sigma^2f}
+R f^{(R-1)/R}=0.}
$$

The resulting feedback is

$$
\boxed{\frac{c^*}{w}=f^{-1/R},\qquad
\frac{\theta^*}{w}=\frac{\mu-r}{R\sigma^2}
+\frac{\alpha}{R\sigma}\frac{f'}f.}
$$

The first portfolio term is myopic, and the second is [intertemporal hedging demand](../../../utility-function.md#intertemporal-hedging-demand).

**Constant market price of risk.** If $\mu-r=\sigma\kappa$ and volatility is nonzero, the portfolio term becomes $p(\kappa f+\alpha f')^2/(2Rf)$, so the magnitude of stock volatility disappears. Applying the [power transformation of a complete-market investment equation](../../../utility-function.md#power-transformation-of-a-complete-market-investment-equation) $f=g^R$ cancels the squared-gradient terms and gives the further reduction

$$
\boxed{\tfrac12\alpha^2g''+
\left(\beta+\frac{p\kappa\alpha}{R}\right)g'
-\gamma_M g+1=0,\qquad
\gamma_M=\frac{\rho-p(r+\kappa^2/(2R))}{R}.}
$$

For $\gamma_M>0$ its economic solution is $g=1/\gamma_M$. Thus

$$
\boxed{V(w,x)=\frac{\gamma_M^{-R}w^p}{p},\qquad
c^*=\gamma_M w,\qquad
\theta^*=\frac{\kappa w}{R\sigma(x)}.}
$$

To see why this solves the [investment-consumption problem](../../../utility-function.md#investment-consumption-problem), optimize directly over [Brownian portfolio exposures](../../../mathematical-finance.md#brownian-portfolio-exposures), writing $y=\sigma(x)\theta$. The [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) equation becomes $dw=y\,dW+(rw+\kappa y-c)dt$, which no longer contains $X$. With nonzero volatility the same admissible exposure processes are available for every factor state, so the attainable wealth-consumption pairs, and therefore the value, are exactly those of the [Merton consumption-investment problem](../../../utility-function.md#merton-consumption-investment-problem). This also excludes extraneous solutions of the linear equation without imposing artificial factor boundary data.

The printed boundedness assumptions do not ensure nonzero volatility or a finite value. The unsimplified [HJB equation](../../../mathematical-optimization.md#hamilton-jacobi-bellman-equation) remains the correct control equation at a zero of $\sigma$. There the hedge term vanishes; if $\mu\ne r$, the riskless excess return gives [arbitrage](../../../mathematical-finance.md#arbitrage) with unrestricted holdings. Under $\mu-r=\sigma\kappa$, a zero-volatility state offers only the bank exposure at that instant. For example $\sigma\equiv0$, $\mu\equiv r$ satisfies this relation for any chosen $\kappa$, but its value uses $\gamma_0=[\rho-pr]/R$, not a fictitious nonzero risk premium. **The constant-value formula using $\kappa$ presupposes access to the Brownian exposure**, with sufficient integrability for the corresponding holdings. Additive utility constants again only shift $V$ by a constant divided by $\rho$.

## 3

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

**Available [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) and the ruin boundary.** Put $h=\bar rD$, the constant interest payment on the fixed loan. The loan principal is already included in available [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth); it is not a growing portfolio holding. Therefore

$$
\boxed{dw=\sigma\theta\,dW+[rw+(\mu-r)\theta-h-c]\,dt,\qquad w_0=x_0+D.}
$$

In particular the interest outflow is $\bar rD$, not $(\bar r-r)D$. Writing $w=x+D$ would instead give net [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) drift $rx+(\mu-r)\theta-(\bar r-r)D-c$, which explains the distinction.

Let $\tau_0$ denote the ruin time, to avoid confusing it with a fixed terminal horizon. The objective stops at $\tau_0$; consequently **the absorbing boundary is $V(0)=0$**, without an obligation to keep financing the loan after ruin. [Dynamic programming](../../../mathematical-optimization.md#dynamic-programming) gives, for $w>0$,

$$
\rho V=(rw-h)V'
+\sup_\theta\{(\mu-r)\theta V'+\tfrac12\sigma^2\theta^2V''\}
+\sup_{c\geq0}\{U(c)-cV'\}.
$$

For increasing strictly [concave](../../../real-analysis.md#concave-function) value, put $z=V'(w)>0$ and use [inverse marginal utility](../../../utility-function.md#inverse-marginal-utility) $I$. The optimal controls and the optimized [HJB equation](../../../mathematical-optimization.md#hamilton-jacobi-bellman-equation) are

$$
c^*=I(z),\qquad \theta^*=-\frac{\kappa}{\sigma}\frac{V'}{V''},\qquad
0=(rw-h)V'-\rho V-\frac{\kappa^2(V')^2}{2V''}+\widetilde U(V'),
$$

where $\widetilde U(z)=\sup_{c\geq0}[U(c)-zc]$. For [CRRA utility](../../../utility-function.md#constant-relative-risk-aversion-utility) with $0<R<1$, write $p=1-R$ and $q=1-1/R<0$. Then

$$
I(z)=z^{-1/R},\qquad \widetilde U(z)=\frac R p z^q.
$$

**Dualization and the printed constant.** Use the convex [wealth-variable Legendre dual](../../../utility-function.md#wealth-variable-legendre-dual)

$$
J(z)=\sup_{w\geq0}[V(w)-zw].
$$

At an interior maximizing [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth), $J'=-w$, $J''=-1/V''>0$ and $V=J-zJ'$. The dual [HJB equation](../../../mathematical-optimization.md#hamilton-jacobi-bellman-equation) is the linear [Euler differential equation](../../../differential-equation.md#cauchy-euler-equation)

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

The appropriate large-wealth condition is the [Merton consumption-investment problem](../../../utility-function.md#merton-consumption-investment-problem) bound

$$
0\leq V(w)\leq \frac{\gamma_M^{-R}}p\,w^p.
$$

Indeed any original control consumes $c+h$ in the debt-free comparison model until ruin, and $U(c+h)\geq U(c)$. Dualizing this bound gives $0\leq J(z)\leq Cz^q$. Because $n<q$, convexity and this upper bound force **$B=0$** as $z\downarrow0$.

At the other endpoint [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) reaches zero. If $z_*=V'(0+)$, the [dual ruin boundary with debt service](../../../utility-function.md#dual-ruin-boundary-with-debt-service) requires

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

Both terms in the bracket are positive, even when $r<0$ and $A<0$. Thus $J''>0$, $-J'$ decreases from infinity to zero as $z$ increases, and the [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) inversion really is unique. The extended dual is continuously differentiable and convex.

There is no additional condition $J''(z_*^-)=0$. In fact

$$
J''(z_*^-)=C(1-q)(m-q)z_*^{q-2}>0.
$$

Available [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) is killed at zero; the portfolio can have a nonzero limiting volatility immediately before ruin. Imposing a reflecting-boundary or zero-curvature condition would solve a different problem.

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

**Verification and transversality.** The candidate is nonnegative, increasing, strictly [concave](../../../real-analysis.md#concave-function) and zero at ruin. Its [HJB equation](../../../mathematical-optimization.md#hamilton-jacobi-bellman-equation) makes the discounted value plus accrued utility a [local supermartingale](../../../martingale.md#local-supermartingale) for every admissible control, and a [local martingale](../../../martingale.md#local-martingale) for the stated feedback. Localization at positive lower and finite upper [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) levels gives the finite-horizon comparison. The [investment value transversality condition](../../../utility-function.md#investment-value-transversality-condition) follows from the same debt-free bound: applying the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $w^p$ and maximizing its risky term gives

$$
\mathbb E[e^{-\rho t}w_t^p\mathbf1_{\{t<\tau_0\}}]
\leq w_0^p e^{-[\rho-p(r+\kappa^2/(2R))]t}
=w_0^p e^{-R\gamma_M t}.
$$

The nonnegative [consumption](../../../mathematical-finance.md#consumption) and debt-service drifts only decrease this bound. Thus the expected terminal candidate tends to zero. The feedback has at most linear growth, including a finite limit as [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) decreases to zero; stopping it at ruin gives an admissible policy. Letting localization levels and then the horizon tend to their limits proves that the candidate is the value, rather than just a formal dual solution. If $D=0$, the absorbing-debt boundary disappears and the ordinary [Merton consumption-investment problem](../../../utility-function.md#merton-consumption-investment-problem) formula is recovered.

**Zero market price of risk.** With $\sigma\ne0$ and $\kappa=0$, the dual equation is first order. If $\rho>r$, the preceding formulas remain valid with $m=\rho/(\rho-r)$ for $r\ne0$, and the logarithmic formula with $b=\rho$ for $r=0$; there is no $B$ term and $\theta^*=0$. The same boundary and transversality argument verifies this deterministic [consumption](../../../mathematical-finance.md#consumption) policy.

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

The two value branches have the same value and derivative at $w_c$. Above $w_c$, hold no stock and consume $\gamma_0(w-h/r)$; the surplus over $h/r$ grows at rate $r-\gamma_0\geq0$. If $\rho=r$, the lower branch is attained by zero stock holding and constant [consumption](../../../mathematical-finance.md#consumption) $ph/R$: [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) solves $\dot w=r(w-w_c)$ until ruin, and direct integration gives $z_cw$.

If $\rho<r$ and $0<w<w_c$, the lower branch is a supremum attained in a limit of increasingly rapid fair stock lotteries between zero and $w_c$, followed by the upper-branch policy on success. The success probability tends to $w/w_c$ and the fixed service cost during the lottery tends to zero. This is possible because unrestricted dollar holdings in the nonzero-volatility stock produce a fair [Brownian motion](../../../brownian-motion.md) exposure even when its excess drift is zero. The supporting linear branch has optimized waiting residual $(r-\rho)z_c(w-w_c)<0$; the fast lotteries, rather than a finite feedback optimizer, supply the missing control limit. The piecewise candidate is [concave](../../../real-analysis.md#concave-function), has nonpositive waiting residual everywhere, and the preceding moment bound still supplies an upper-bound verification. **This degenerate case can have a supremum without an ordinary maximizing strategy.**

## 4

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

**Pricing kernel and replication.** In the nondegenerate [Black-Scholes model](../../../mathematical-finance.md#black-scholes-model), put $\kappa=(\mu-r)/\sigma$ and normalize the [state-price density](../../../mathematical-finance.md#state-price-density) by $\zeta_0=1$. The process is

$$
\boxed{\zeta_t=\exp\{-rt-\kappa W_t-\tfrac12\kappa^2t\},\qquad
d\zeta_t=-\zeta_t(r\,dt+\kappa\,dW_t).}
$$

The density $e^{rt}\zeta_t$ changes probability to the [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure). Under that measure $W_t+\kappa t$ is a [Brownian motion](../../../brownian-motion.md) and the stock drift is $r$. Thus an integrable [contingent claim](../../../mathematical-finance.md#contingent-claim) $H$ has time-$t$ price

$$
\boxed{P_t=\frac{\mathbb E[\zeta_T H\mid\mathcal F_t]}{\zeta_t}
=e^{-r(T-t)}\mathbb E^{\mathbb Q}[H\mid\mathcal F_t].}
$$

In the usual augmented [natural Brownian filtration](../../../brownian-motion.md#natural-brownian-filtration), the [Brownian martingale representation theorem](../../../brownian-motion.md#brownian-martingale-representation-theorem) supplies a [replicating strategy](../../../mathematical-finance.md#replicating-strategy); this is the [complete market](../../../mathematical-finance.md#complete-market) assumption. For a nonnegative [admissible trading strategy](../../../mathematical-finance.md#admissible-trading-strategy) without intermediate [consumption](../../../mathematical-finance.md#consumption), the [state-price budget constraint](../../../mathematical-finance.md#state-price-budget-constraint) is $\mathbb E[\zeta_Tw_T]\leq w_0$, with equality for a fully invested replicated claim. In particular

$$
\mathbb E\zeta_T=e^{-rT},\qquad \mathbb E[\zeta_TS_T]=S_0.
$$

**Feasibility and the largest slope.** First take the intended regime $r>0$, $T>0$, $w_0,S_0>0$, and the usual nonnegative [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) constraint. The [terminal wealth floor](../../../utility-function.md#terminal-wealth-floor) is

$$
\xi=w_0+\alpha(S_T-S_0).
$$

For any feasible claim the [state-price budget constraint](../../../mathematical-finance.md#state-price-budget-constraint) implies

$$
w_0\geq\mathbb E[\zeta_Tw_T]\geq
\mathbb E[\zeta_T\xi]
=w_0e^{-rT}+\alpha S_0(1-e^{-rT}).
$$

Therefore $\alpha\leq w_0/S_0$. Conversely, when $0\leq\alpha\leq w_0/S_0$, hold $\alpha$ shares and put the remaining $w_0-\alpha S_0$ in the [continuous-time bank account](../../../mathematical-finance.md#continuous-time-bank-account). Its terminal [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) is

$$
\alpha S_T+(w_0-\alpha S_0)e^{rT}
\geq\alpha S_T+(w_0-\alpha S_0)=\xi.
$$

Hence

$$
\boxed{\bar\alpha=\frac{w_0}{S_0}.}
$$

At equality, $\xi=\bar\alpha S_T$ has cost exactly $w_0$. Positivity of the [state-price density](../../../mathematical-finance.md#state-price-density) forces $w_T=\bar\alpha S_T$ almost surely: any strict improvement would cost more. **Invest all initial [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) in $w_0/S_0$ shares and hold them until $T$.**

**Optimal payoff below the feasibility limit.** For $\alpha<\bar\alpha$ the floor is strictly positive, and its price is strictly less than $w_0$. Assume the [utility function](../../../utility-function.md) is increasing, differentiable and strictly [concave](../../../real-analysis.md#concave-function), satisfies the [Inada conditions](../../../utility-function.md#inada-conditions), and has the integrability needed for the finite-budget optimization. These are the usual hypotheses implicit in using [inverse marginal utility](../../../utility-function.md#inverse-marginal-utility). For each positive multiplier $\lambda$, maximize

$$
U(y)-\lambda\zeta_Ty\qquad\text{over }y\geq\xi
$$

separately in every state. Its derivative decreases through zero at $I(\lambda\zeta_T)$, so the [floored marginal utility optimizer](../../../utility-function.md#floored-marginal-utility-optimizer) is

$$
\boxed{w_T^*=\max\{w_0+\alpha(S_T-S_0),\,I(\lambda\zeta_T)\}.}
$$

The multiplier is characterized by

$$
\boxed{\mathbb E\!\left[\zeta_T\max\{\xi,I(\lambda\zeta_T)\}\right]=w_0,\qquad \lambda>0.}
$$

Under the stated integrability hypotheses the left side is continuous and decreasing, tends to the floor cost as $\lambda\uparrow\infty$, and tends to infinity as $\lambda\downarrow0$. It is strictly decreasing wherever it exceeds the floor cost: on the event where the inverse-marginal-utility payoff exceeds the floor, a larger multiplier strictly reduces that payoff. Therefore the budget determines a unique finite multiplier. For [CRRA utility](../../../utility-function.md#constant-relative-risk-aversion-utility) the [inverse marginal utility](../../../utility-function.md#inverse-marginal-utility) is $I(y)=y^{-1/R}$; lognormal moments provide the needed integrability.

For completeness, pointwise maximality gives, for any feasible competing terminal [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) $Y$,

$$
U(Y)-\lambda\zeta_TY
\leq U(w_T^*)-\lambda\zeta_Tw_T^*.
$$

Taking expectations and using $\mathbb E[\zeta_TY]\leq w_0=\mathbb E[\zeta_Tw_T^*]$ proves optimality. Strict [concavity](../../../real-analysis.md#concave-function) gives uniqueness of the terminal claim. Its price process

$$
w_t^*=\frac{\mathbb E[\zeta_Tw_T^*\mid\mathcal F_t]}{\zeta_t}
$$

is nonnegative and starts from $w_0$; [claim replication](../../../mathematical-finance.md#claim-replication) therefore turns the payoff optimizer into an admissible portfolio.

**What the missing interest-rate hypothesis changes.** The PDF does not explicitly assume $r>0$ or give the utility and admissibility hypotheses above. These omissions matter. At $r=0$, under nonnegative admissibility, the largest feasible slope remains $w_0/S_0$: for larger slopes the positive-part floor costs strictly more than $w_0$, since $S_T$ has support $(0,\infty)$. But every $\alpha\leq w_0/S_0$ already gives floor cost exactly $w_0$, so the only feasible terminal claim is $\xi$. There is no spare budget for an inverse-marginal-utility improvement. For example $\alpha=0$, $\kappa\ne0$ and [CRRA utility](../../../utility-function.md#constant-relative-risk-aversion-utility) make $\mathbb E[\zeta_T\max\{w_0,I(\lambda\zeta_T)\}]>w_0$ for every finite $\lambda$. The prescribed positive finite multiplier then does not exist.

For negative $r$, nonnegative admissibility requires the effective floor $\xi_+=\max\{\xi,0\}$. Define its cost

$$
G(\alpha)=\mathbb E[\zeta_T(w_0+\alpha(S_T-S_0))_+].
$$

This is continuous and convex. For $\alpha\leq w_0/S_0$ it equals $w_0e^{-rT}+\alpha S_0(1-e^{-rT})$, exceeding $w_0$ below the endpoint. At $\alpha_0=w_0/S_0$, $G(\alpha_0)=w_0$ and $G'(\alpha_0)=S_0(1-e^{-rT})<0$. Above that endpoint the lognormal stock gives strict convexity, and $G(\alpha)\to\infty$. Thus there is a unique second root $\alpha_1>\alpha_0$ of $G(\alpha_1)=w_0$, the feasible slopes are $[\alpha_0,\alpha_1]$, and the largest is $\alpha_1$. Equivalently, for $\alpha>\alpha_0$ the floor price is $\alpha$ times the [European call option](../../../mathematical-finance.md#european-call-option) price with strike $S_0-w_0/\alpha$. At the upper endpoint replicate $\xi_+$; in the interval with strict budget slack the same [floored marginal utility optimizer](../../../utility-function.md#floored-marginal-utility-optimizer) applies with $\xi_+$.

If instead [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) may be negative and utility is defined on all real [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth), the floor itself has its affine replication cost: at $r=0$ every slope is feasible, and at negative $r$ every $\alpha\geq w_0/S_0$ is feasible. There is then no largest finite slope. **The intended stock-only endpoint and strict-slack optimizer use positive interest and standard nonnegative admissibility.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
