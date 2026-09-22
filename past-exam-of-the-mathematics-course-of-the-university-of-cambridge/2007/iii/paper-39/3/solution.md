<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Each marginal is a [Bessel process](../../../../../bessel-process.md) of [dimension](../../../../../dimension-vector-space.md) $\delta=1+2a\in(1,2)$, but finite lifetime can also be proved directly. Apply the [Itô formula](../../../../../ito-s-lemma.md) before $X$ reaches zero:

$$
\log X_t=\log x+\int_0^tX_s^{-1}\,dB_s+
\left(a-\frac12\right)\int_0^tX_s^{-2}\,ds.
$$

With clock $u(t)=\int_0^tX_s^{-2}ds$, the [Itô integral](../../../../../ito-integral.md) is a [Brownian motion](../../../../../brownian-motion-split.md) $W_u$. The inverse clock satisfies

$$
X_{t(u)}=x e^{W_u-(1/2-a)u},\qquad
 t(u)=x^2\int_0^u e^{2W_v-(1-2a)v}\,dv.
$$

The clock runs through all $u\geq0$ up to the maximal lifetime: a finite terminal clock would leave $X$ at a finite positive limit, allowing continuation, or, at an infinite physical lifetime, would make its clock grow at a positive rate, a contradiction. There is no finite-time explosion to infinity; for example $dX_t^2=2X_t\,dB_t+(1+2a)dt$ and localization bounds the probability of reaching arbitrarily large levels on a fixed time interval. Since $W_u/u\to0$ almost surely and $1-2a>0$, the last exponential integral has finite limit, while $X_{t(u)}\to0$. Therefore

$$
\boxed{\zeta=x^2\int_0^\infty e^{2W_v-(1-2a)v}\,dv<\infty\quad\text{almost surely}.}
$$

The same argument applies to $Y$, whose noise $-B$ is also [Brownian motion](../../../../../brownian-motion-split.md), so its lifetime is finite too. No [independence](../../../../../independent-random-variables.md) between the two lifetimes is being claimed.

Set $S=X+Y$ and $U=Y/S$ before $T=\zeta\wedge\tau$. [Brownian motion](../../../../../brownian-motion-split.md) terms cancel in the sum:

$$
dS_t=a\left(\frac1{X_t}+\frac1{Y_t}\right)dt,
\qquad S_t\geq x+y>0.
$$

Thus simultaneous extinction is impossible. At the finite first lifetime, precisely one coordinate is zero and the other remains positive. Because $S$ has finite variation, differentiating the ratio gives

$$
dU_t=-\frac1{S_t}\,dB_t
+\frac{a(1-2U_t)}{S_t^2U_t(1-U_t)}dt.
$$

After clock change $v=\int_0^tS_s^{-2}ds$, its generator is

$$
\mathcal L=\frac12\frac{d^2}{du^2}
+\frac{a(1-2u)}{u(1-u)}\frac d{du}.
$$

A [scale function of a one-dimensional diffusion](../../../../../scale-function-stochastic-processes.md) $H$ solves $\mathcal LH=0$, so

$$
\frac{H''}{H'}=-2a\frac{1-2u}{u(1-u)},\qquad
H'(u)=C u^{-2a}(1-u)^{-2a}.
$$

Both endpoint singularities are integrable since $a<1/2$. Normalize $H(0)=0,H(1)=1$ to obtain

$$
H(u)=\frac{\displaystyle\int_0^u v^{-2a}(1-v)^{-2a}dv}
{\displaystyle\int_0^1 v^{-2a}(1-v)^{-2a}dv}.
$$

The [Itô formula](../../../../../ito-s-lemma.md) makes $H(U_{t\wedge T})$ a bounded [martingale](../../../../../martingale-split.md), first by localization away from the endpoints and then by [bounded convergence theorem](../../../../../bounded-convergence-theorem.md). Its terminal value is one on $\{\zeta<\tau\}$, when $U_T=1$, and zero on the opposite event, when $U_T=0$. [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) therefore proves the [oppositely driven Bessel exit probability](../../../../../oppositely-driven-bessel-exit-probability.md)

$$
\boxed{\mathbb P(\zeta<\tau)=
\frac1{\mathrm B(1-2a,1-2a)}\int_0^{y/(x+y)}\frac{du}{u^{2a}(1-u)^{2a}},
\qquad c_a=\frac{\Gamma(2-4a)}{\Gamma(1-2a)^2}.}
$$

Here $\mathrm B$ is the [beta function](../../../../../beta-function.md) and $\Gamma$ is the [Gamma function](../../../../../gamma-function.md).

**The integral printed in the question is incorrect for general $a$.** Its first exponent is $2-4a$, whereas the two coupled equations give $2a$. At $a=1/4$, which lies in the allowed interval, its integral from zero diverges for every positive upper limit; no finite normalizing constant gives a probability. Moreover exchanging $X$ and $Y$ while changing $B$ to $-B$ shows that at $x=y$ the probability must be $1/2$. The corrected symmetric integral has this value for every $a\in(0,1/2)$, whereas the printed asymmetric normalized integral generally does not. For $a>1/4$, even when the printed integral converges, its [derivative](../../../../../derivative.md) density $H_{\mathrm{print}}'(u)\propto u^{-(2-4a)}(1-u)^{-2a}$ satisfies

$$
\frac{\mathcal LH_{\mathrm{print}}}{H_{\mathrm{print}}'}=\frac{3a-1}{u},
$$

so it is harmonic for the required exit problem only at $a=1/3$. The two exponents agree exactly at that value.

To relate that value to [percolation](../../../../../percolation-theory.md), write the two [SLE](../../../../../schramm-loewner-evolution.md) [boundary](../../../../../boundary-of-a-set.md) gaps as $g_t(x)-\xi_t$ and $\xi_t-g_t(-y)$. In Brownian-time units $s=\kappa t$, they have the displayed coupled equations with $a=2/\kappa$, after reversing the [Brownian motion](../../../../../brownian-motion-split.md) sign. Hence $a=1/3$ corresponds to $\kappa=6$. The event is that the positive marked point $x$ is swallowed before the negative marked point $-y$.

For a quadrilateral with [boundary](../../../../../boundary-of-a-set.md) points in the order $(-y,0,x,\infty)$, its conformal [cross-ratio](../../../../../cross-ratio.md) coordinate is $u=y/(x+y)$. In the critical [percolation](../../../../../percolation-theory.md) exploration, wire the arcs $(-y,0)$ and $(x,\infty)$ blue and the other two arcs yellow. Exploration from zero, stopped when one of the two marked sides is swallowed, detects a blue crossing between those two blue arcs exactly in the event just computed. The continuum exploration has the SLE6 law; its [Locality property of SLE](../../../../../locality-property-of-sle.md) lets one stop the ordinary chordal exploration before the distant [boundary](../../../../../boundary-of-a-set.md) colors affect it. Thus the crossing probability is

$$
\boxed{\frac{\Gamma(2/3)}{\Gamma(1/3)^2}\int_0^{y/(x+y)}[u(1-u)]^{-2/3}du,}
$$

the [Cardy boundary crossing formula](../../../../../cardy-boundary-crossing-formula.md). This is the rigorous scaling-limit formula for critical [site percolation](../../../../../site-percolation-split.md) on the triangular lattice; applying it to other critical planar models requires the corresponding universality assumption. At this [percolation](../../../../../percolation-theory.md) value of $a$, the printed integral is already the correct one.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
