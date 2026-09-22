<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $I=(U')^{-1}$ be the [inverse marginal utility](../../../../../inverse-marginal-utility.md). The [derivative](../../../../../derivative.md) $U'$ is continuous and strictly decreasing: concavity makes it nonincreasing, and equality at two distinct points would make $U$ affine between them, contradicting [strict concavity](../../../../../strict-concavity.md). The [Inada conditions](../../../../../inada-conditions.md) therefore make $U'$ a bijection from $(0,\infty)$ onto $(0,\infty)$. For each $y>0$, the [derivative](../../../../../derivative.md) of $U(x)-xy$ is positive below $I(y)$ and negative above it. Consequently its unique global maximum is finite and

$$
V(y)=U(I(y))-yI(y).
$$

There is no need to differentiate $I$ to find the first [derivative](../../../../../derivative.md) of this [utility conjugate](../../../../../utility-conjugate.md). Comparing the maxima at $y$ and $y+h$ gives, for $h>0$,

$$
-hI(y)\leq V(y+h)-V(y)\leq-hI(y+h).
$$

Continuity of $I$, together with the corresponding inequalities for $h<0$, gives

$$
\boxed{V'(y)=-I(y),\qquad V'(0+)=-\infty,\qquad V'(\infty)=0.}
$$

Thus $V$ is strictly decreasing and [strictly convex](../../../../../strictly-convex-function.md), since its [derivative](../../../../../derivative.md) is strictly increasing. This proves all the asserted properties except the second [differentiability](../../../../../differentiability.md), which does not follow from the printed hypotheses.

Here is an explicit [Inada utility with vanishing curvature](../../../../../inada-utility-with-vanishing-curvature.md). Put

$$
w(s)=\frac{(s-1)^2}{s^2(s+1)^2},\qquad p(x)=\int_x^\infty w(s)\,ds=\frac1x+\frac4{x+1}+4\log\frac{x}{x+1},\qquad U(x)=\int_1^x p(r)\,dr.
$$

The positive integral defining $p$ makes $U$ strictly increasing. Also $p'=-w$ is negative except at one point, so $p$ is strictly decreasing and $U$ is [strictly concave](../../../../../strictly-concave-function.md). Near zero $w(s)$ is asymptotic to $s^{-2}$, and at infinity it is asymptotic to $s^{-2}$; thus $p(0+)=\infty$ and $p(\infty)=0$. This smooth [utility function](../../../../../utility-function-split.md) satisfies every printed positive-domain assumption, but $U''(1)=0$. At $y_0=p(1)=3-4\log2$, differentiability of $I$ would imply, by differentiating $p(I(y))=y$,

$$
0\cdot I'(y_0)=1,
$$

which is impossible. Hence $V'=-I$ has no finite [derivative](../../../../../derivative.md) there. More explicitly, $p(x)-p(1)=-(x-1)^3/12+o((x-1)^3)$, so its [inverse function](../../../../../inverse-function.md) has a cube-root singularity. **The twice-differentiable conclusion is false as printed.** With the additional assumption $U''(x)<0$ everywhere, the [inverse function theorem](../../../../../inverse-function-theorem.md) proves the intended [dual differentiability with nonvanishing utility curvature](../../../../../dual-differentiability-with-nonvanishing-utility-curvature.md):

$$
\boxed{V''(y)=-\frac1{U''(I(y))}>0.}
$$

For the financial assertions, use the positive-wealth [admissible trading strategy](../../../../../admissible-trading-strategy.md) class appropriate to the positive-domain [utility function](../../../../../utility-function-split.md), and expectations for which the expressions are defined. A normalized terminal [state-price density](../../../../../state-price-density.md) satisfies $Z_N>0$, $\mathbb EZ_N=1$, and defines an [equivalent martingale measure](../../../../../risk-neutral-measure.md) $Q$ by $dQ=Z_N\,dP$. A [self-financing portfolio](../../../../../self-financing-portfolio.md) obeys

$$
X_n=x+\sum_{k=0}^{n-1}\pi_k\cdot(S_{k+1}-S_k),
$$

where the holdings are measurable before the next price increment. Under $Q$ the gains are a [martingale](../../../../../martingale-split.md) when integrable; for the usual lower-bounded admissible class, localization gives a [supermartingale](../../../../../supermartingale.md). In particular the [state-price budget constraint](../../../../../state-price-budget-constraint.md) is $\mathbb E[Z_NX_N]\leq x$. The positive-domain qualification matters: assumptions only on $U$ at positive arguments do not control its values at nonpositive wealth.

The definition of the [utility conjugate](../../../../../utility-conjugate.md) gives the pointwise inequality

$$
U(X_N)\leq V(yZ_N)+yZ_NX_N.
$$

Taking expectations, using the [state-price budget constraint](../../../../../state-price-budget-constraint.md), and then taking the supremum over strategies gives $u(x)\leq\mathbb EV(yZ_N)+yx$ for every $y>0$ and every [state-price density](../../../../../state-price-density.md). Taking the two infima proves the [utility duality with martingale deflators](../../../../../utility-duality-with-martingale-deflators.md) upper bound:

$$
\boxed{u(x)\leq\inf_{y>0}\{v(y)+xy\}.}
$$

If an expectation is infinite, use the same inequality in the extended-real sense whenever the negative parts make it well defined; no subtraction of two infinities is needed.

A [complete market](../../../../../complete-market.md) is one in which every terminal [contingent claim](../../../../../contingent-claim.md) in the specified claim class is attainable by a [self-financing portfolio](../../../../../self-financing-portfolio.md). Bounded terminal claims suffice for the uniqueness argument. In the standard finite-horizon discrete-time market, absence of [arbitrage](../../../../../arbitrage.md) gives existence of an [equivalent martingale measure](../../../../../risk-neutral-measure.md) by the [fundamental theorem of asset pricing](../../../../../fundamental-theorem-of-asset-pricing.md). To prove uniqueness, let $Z_N$ and $\widetilde Z_N$ be two normalized [state-price densities](../../../../../state-price-density.md). Every bounded claim $H$ has a replicating price $p(H)$, and its replication has the same price under either [equivalent martingale measure](../../../../../risk-neutral-measure.md):

$$
\mathbb E[Z_NH]=p(H)=\mathbb E[\widetilde Z_NH].
$$

Take $H=\mathbf1_A$ for every terminal event $A$. The integrable difference $Z_N-\widetilde Z_N$ has zero integral over every event, hence vanishes almost surely: its positive and negative sets would otherwise give a nonzero integral. **The normalized terminal state-price density is unique up to null sets.** Its density process is then uniquely $Z_n=\mathbb E[Z_N\mid\mathcal F_n]$. This uses the usual pricing replication class, where bounded claims have bounded replicating value processes; arbitrary doubling strategies are not an admissible definition of completeness.

For [logarithmic utility](../../../../../logarithmic-utility.md), direct maximization gives $V(y)=-\log y-1$. In the [complete market](../../../../../complete-market.md), write $Z=Z_N$. The unique-density [utility conjugate](../../../../../utility-conjugate.md) bound is minimized at $y=1/x$, giving

$$
u(x)\leq\log x-\mathbb E\log Z.
$$

The candidate terminal [portfolio wealth](../../../../../portfolio-wealth.md) is $H^*=x/Z$, whose cost is exactly $\mathbb E[ZH^*]=x$. If completeness includes nonnegative $Q$-integrable claims, it is replicable and attains the bound. There is also an approximation proof using only bounded-claim completeness. Define

$$
b_n=\mathbb E\frac{Z}{Z\vee n^{-1}},\qquad H_n=\frac{x}{b_n(Z\vee n^{-1})}.
$$

Then $0<b_n\leq1$, $b_n\uparrow1$, $H_n$ is positive and bounded, and $\mathbb E[ZH_n]=x$. Replicating $H_n$ therefore gives an admissible terminal claim of initial cost $x$. Since $\mathbb E(\log Z)^+\leq\mathbb EZ=1$, the negative parts of $-\log(Z\vee n^{-1})$ have an integrable common bound. [Monotone convergence](../../../../../monotone-convergence-theorem.md) after adding this lower bound gives

$$
\mathbb E\log H_n=\log x-\log b_n-\mathbb E\log(Z\vee n^{-1})\longrightarrow\log x-\mathbb E\log Z.
$$

Consequently the [logarithmic terminal wealth in a complete market](../../../../../logarithmic-terminal-wealth-in-a-complete-market.md) is

$$
\boxed{u(x)=\log x-\mathbb E\log Z_N,\qquad H^*=\frac{x}{Z_N}.}
$$

The value may be $+\infty$ if $\mathbb E(\log Z_N)^-=\infty$; the displayed formula remains meaningful, while attainment by $H^*$ depends on the precise admissible claim class.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
