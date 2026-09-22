<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The PDF prints $w_0=0$ in the conditioning of the value function. Taken literally, nonnegative wealth and the [state-price budget constraint](../../../../../state-price-budget-constraint.md) force both wealth and consumption to remain zero, and the utility for $R>1$ has value $-\infty$. The meaningful value function underlying the subsequent requests uses $w_0=w>0$; the following calculation makes that source correction explicit.

Write $h_t=\bar c_t>0$. Differentiating the [exponentially weighted consumption habit](../../../../../exponentially-weighted-consumption-habit.md) gives **the habit-state dynamics**

$$
\boxed{dh_t=\lambda(c_t-h_t)\,dt.}
$$

Multiplying initial wealth, initial habit, investments, and consumption by $a>0$ multiplies the wealth and habit paths by $a$. The ratio $c/h$ is unchanged, while $U(ac)=a^{1-R}U(c)$. Thus **the homogeneous value is**

$$
\boxed{V(w,h)=h^{1-R}v(w/h).}
$$

This is a [multiplicative habit utility](../../../../../multiplicative-habit-utility.md) model: higher habit makes utility more negative at fixed consumption.

Set $S=R+\alpha>1$, $K=(S-1)/(R-1)>0$, and $\kappa=(\mu-r)/\sigma$. The instantaneous reward is

$$
g(c,h)=\frac{h^\alpha c^{1-S}}{1-R}
=K h^\alpha\frac{c^{1-S}}{1-S}.
$$

For smooth increasing, strictly [concave](../../../../../concave-function.md) wealth value, the [Hamilton-Jacobi-Bellman equation](../../../../../hamilton-jacobi-bellman-equation.md) is

$$
0=-\rho V+rwV_w-\lambda hV_h
+\sup_{\theta\in\mathbb R}
\left\{\tfrac12\sigma^2\theta^2V_{ww}+(\mu-r)\theta V_w\right\}
+\sup_{c>0}\{g(c,h)-c(V_w-\lambda V_h)\}.
$$

The [effective consumption shadow price with habit](../../../../../effective-consumption-shadow-price-with-habit.md) changes from $V_w$ to $D=V_w-\lambda V_h$. For $D>0$, consumption maximization gives

$$
c^*=(Kh^\alpha/D)^{1/S},\qquad
\sup_{c>0}\{g(c,h)-Dc\}
=-\frac S{S-1}(Kh^\alpha)^{1/S}D^{1-1/S}.
$$

For $D<0$ the supremum is infinite, and for $D=0$ its zero supremum is approached only as consumption tends to infinity; a finite interior optimum therefore requires $D>0$. The portfolio maximum is $-\kappa^2V_w^2/(2V_{ww})$.

Let $x=w/h$, $z=v'(x)$, and define

$$
d(x)=(1+\lambda x)v'(x)-\lambda(1-R)v(x),\qquad
H(d)=-\frac S{S-1}K^{1/S}d^{1-1/S}.
$$

The [homogeneity](../../../../../homogeneity.md) derivatives are

$$
V_w=h^{-R}v',\quad V_{ww}=h^{-R-1}v'',\quad
V_h=h^{-R}[(1-R)v-xv'].
$$

Consequently $D=h^{-R}d(x)$, and the reward conjugate is $h^{1-R}H(d(x))$. **The reduced habit equation is**

$$
\boxed{(r+\lambda)xv'-[\rho+\lambda(1-R)]v
-\tfrac12\kappa^2\frac{(v')^2}{v''}+H(d(x))=0.}
$$

For completeness its feedback controls are $c^*/h=(K/d)^{1/S}$ and $\theta^*/h=-(\mu-r)v'/(\sigma^2v'')$.

The [wealth-variable Legendre dual](../../../../../wealth-variable-legendre-dual.md) $J(z)=v(x)-xz$ satisfies $J'=-x$, $J''=-1/v''$, and $v=J-zJ'$. The effective shadow price becomes

$$
\mathcal D(z)=z-\lambda RzJ'(z)+\lambda(R-1)J(z).
$$

Therefore **the [dual equation for multiplicative habit investment](../../../../../dual-equation-for-multiplicative-habit-investment.md) is**

$$
\boxed{\tfrac12\kappa^2z^2J''
+(\rho-r-\lambda R)zJ'
-[\rho+\lambda(1-R)]J
-\frac S{S-1}K^{1/S}
\left[z-\lambda RzJ'+\lambda(R-1)J\right]^{1-1/S}=0,}
$$

with $\mathcal D>0$. The dependence of the reward conjugate on $J$ and $J'$ is the remaining nonlinearity.

When $\lambda=0$, habit is fixed and the equation becomes **a linear Euler equation**

$$
\boxed{\tfrac12\kappa^2z^2J''+(\rho-r)zJ'-\rho J+H(z)=0.}
$$

The forcing is a pure power $z^{1-1/S}$. Thus the [Euler differential equation](../../../../../cauchy-euler-equation.md) method gives a power particular solution plus the two homogeneous characteristic powers in the nondegenerate case. Economically, this is the [Merton consumption-investment problem](../../../../../merton-consumption-investment-problem.md) with effective relative risk aversion $S=R+\alpha$ and a constant reward multiplier. Writing

$$
\delta_S=\frac{\rho-(1-S)[r+\kappa^2/(2S)]}{S}>0,
$$

its value and controls are

$$
\boxed{v(x)=\frac{K\delta_S^{-S}}{1-S}x^{1-S},\qquad
c^*=\delta_S w,\qquad \theta^*=\frac{\mu-r}{S\sigma^2}w.}
$$

Indeed $H(z)/\delta_S$ solves the dual equation, since its characteristic polynomial at $1-1/S$ equals $-\delta_S$. Unlike the $\lambda>0$ case, the fixed habit creates no feedback coupling between the dual value and the shadow price of consumption.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
