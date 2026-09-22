<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [SIPV model](../../../../../symmetric-independent-private-values-model.md) concerns a fixed number of bidders competing for one object. Each bidder knows their own private valuation; the value of winning depends on that valuation alone. Valuations are [independent random variables](../../../../../independent-random-variables.md) with the same atomless distribution $F$, known to everyone, and bidders have identical roles and access to the same strategies. The standard [revenue equivalence](../../../../../revenue-equivalence.md) setting also assumes [risk neutrality](../../../../../risk-neutrality.md), [quasilinear utility](../../../../../quasilinear-utility.md), and noncooperative bidding: expected utility is valuation times winning probability minus expected payment.

The [revenue equivalence theorem](../../../../../revenue-equivalence.md) states that auctions with the same equilibrium allocation probability $p(v)$ for each type and the same expected utility for the lowest type have the same expected payment by each type, and therefore the same expected seller revenue. In particular, if the object goes to the highest valuation and the lowest type has zero expected utility, then all such auctions have the same expected revenue. In a strictly increasing symmetric equilibrium, $p(v)=F(v)^{n-1}$.

For a bidder of valuation $v$, the profit as a function of winning probability is $vp-e(p)$. At an interior [stationary point](../../../../../stationary-point.md) $p(v)$,

$$
\frac{d}{dp}\bigl(vp-e(p)\bigr)=v-e'(p)=0.
$$

The [chain rule](../../../../../chain-rule.md) then gives the first two identities:

$$
\boxed{e'(p(v))=v,\qquad
\frac{d}{dv}e(p(v))=v\,p'(v).}
$$

Integrating from zero and using [integration by parts](../../../../../integration-by-parts.md) gives the [interim payment identity](../../../../../interim-payment-identity.md)

$$
e(p(v))=e(p(0))+\int_0^v w p'(w)\,dw
=e(p(0))+vp(v)-\int_0^v p(w)\,dw.
$$

With the usual zero-payment normalization $e(p(0))=0$, this becomes

$$
\boxed{e(p(v))=vp(v)-\int_0^v p(w)\,dw.}
$$

Stationarity alone does not determine the integration constant: a fixed participation fee would add that constant. The stated formula uses the lowest-type normalization from [revenue equivalence](../../../../../revenue-equivalence.md).

For the [lowest-price auction](../../../../../lowest-price-auction.md) with independent [uniform distributions](../../../../../continuous-uniform-distribution.md) on $[0,1]$, consider the symmetric increasing equilibrium, so that $p(v)=v^{n-1}$. The zero type can bid zero, lose almost surely, and pay nothing. The [interim payment identity](../../../../../interim-payment-identity.md) therefore yields

$$
e(p(v))=v^n-\int_0^v w^{n-1}\,dw
=\frac{n-1}{n}v^n.
$$

Sum this expected payment over the $n$ bidders and average over their [uniform distributions](../../../../../continuous-uniform-distribution.md):

$$
\boxed{\mathbb E[\text{seller revenue}]
=n\int_0^1\frac{n-1}{n}v^n\,dv
=\frac{n-1}{n+1}.}
$$

This uses $n\geq2$, as appropriate for this auction format.

For three bidders, assume the common bid is $Av$ with $A>0$. If a bidder deviates to $Az$, $0\leq z\leq1$, they win precisely when both opposing valuations $u,w$ are below $z$. On that event they pay $A\min(u,w)$, so their expected payment and profit are

$$
e_z=A\int_0^z\int_0^z\min(u,w)\,du\,dw=\frac A3z^3,
\qquad
U(v,z)=vz^2-\frac A3z^3.
$$

For $0<v<1$, stationarity at $z=v$ gives $2v^2-Av^2=0$, hence

$$
\boxed{A=2.}
$$

This is a global [best response](../../../../../best-response.md), not merely a [stationary point](../../../../../stationary-point.md): for $A=2$, $\partial U/\partial z=2z(v-z)$ is positive for $0<z<v$ and negative for $v<z\leq1$. Any bid above $2$ gives the same sure-win payment as $z=1$ and cannot improve the payoff.

The [uniform lowest-price auction equilibrium](../../../../../uniform-lowest-price-auction-equilibrium.md) also verifies the revenue calculation constructively for any $n\geq2$. If opponents bid $(n-1)u$, a deviation to $(n-1)z$ has profit

$$
U(v,z)=vz^{n-1}-\frac{n-1}{n}z^n,
\qquad
\frac{\partial U}{\partial z}=(n-1)z^{n-2}(v-z).
$$

Thus $z=v$ is optimal and $b(v)=(n-1)v$ is a symmetric [Bayesian Nash equilibrium](../../../../../bayesian-nash-equilibrium.md). The realized price is $(n-1)$ times the minimum valuation; this [order statistic](../../../../../order-statistic.md) has expectation $\int_0^1(1-t)^n\,dt=1/(n+1)$, giving the same expected revenue.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
