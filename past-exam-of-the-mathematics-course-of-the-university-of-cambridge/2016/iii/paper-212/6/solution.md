<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use the standard [risk-neutral](../../../../../risk-neutrality.md) [quasilinear utility](../../../../../quasilinear-utility.md) model: utility is value received minus payment. A bidder may abstain for utility zero, payments to the seller are nonnegative, and the zero-value type has utility zero. The last normalization is necessary for the requested revenue formula; if arbitrary subsidies were allowed, an additive payment constant would remain undetermined. The [independent private values model](../../../../../independent-private-values-model.md) is symmetric, and each bidder has a [unit-demand valuation](../../../../../unit-demand-valuation.md) in the two-item part. Participation satisfies [individual rationality](../../../../../individual-rationality.md).

Let $G(\theta)$ be the interim probability of receiving an item and $m(\theta)$ the interim expected payment of a type $\theta$. Write $u(\theta)=\theta G(\theta)-m(\theta)$. By mimicking the [Bayesian Nash equilibrium](../../../../../bayesian-nash-equilibrium.md) bid of a type $z$, a type $\theta$ could obtain utility $\theta G(z)-m(z)$. Equilibrium therefore gives, for $\theta>z$,

$$
G(z)\leq\frac{u(\theta)-u(z)}{\theta-z}\leq G(\theta).
$$

The lower inequality uses type $\theta$'s incentive constraint, and the upper uses type $z$'s. Since $G$ is continuous in these auctions, the inequalities give $u'(\theta)=G(\theta)$. With $u(0)=0$,

$$
\boxed{u(\theta)=\int_0^\theta G(t)dt,\qquad m(\theta)=\theta G(\theta)-\int_0^\theta G(t)dt.}
$$

This is the [interim payment identity](../../../../../interim-payment-identity.md) underlying [revenue equivalence](../../../../../revenue-equivalence.md).

For one item, independence and the [uniform distribution](../../../../../continuous-uniform-distribution.md) give $G(\theta)=\theta^{n-1}$: all other values must be below $\theta$. Hence **the expected payment from a bidder conditional on its value is**

$$
\boxed{m(\theta)=\theta^n-\frac{\theta^n}{n}=\frac{n-1}{n}\theta^n.}
$$

This is an unconditional-in-winning interim payment, not the amount paid conditional on winning. In the [first-price sealed-bid auction](../../../../../first-price-sealed-bid-auction.md), $m(\theta)=b(\theta)G(\theta)$, so **the [Bayesian Nash equilibrium](../../../../../bayesian-nash-equilibrium.md) bid is**

$$
\boxed{b(\theta)=\frac{n-1}{n}\theta,}
$$

with $b(0)=0$. For $n=1$, the seller's revenue is zero and a zero bid suffices under the stipulated allocation rule.

For two items and three unit-demand bidders, a type $\theta$ wins if at most one of the other two values exceeds it. Therefore

$$
G(\theta)=\theta^2+2\theta(1-\theta)=2\theta-\theta^2,\qquad u(\theta)=\theta^2-\frac{\theta^3}{3}.
$$

The [interim payment identity](../../../../../interim-payment-identity.md) gives $m(\theta)=\theta^2-2\theta^3/3$. Dividing by the winning probability gives **the symmetric [Bayesian Nash equilibrium](../../../../../bayesian-nash-equilibrium.md) bid**

$$
\boxed{b(\theta)=\frac{\theta^2-2\theta^3/3}{2\theta-\theta^2}=\frac{3\theta-2\theta^2}{6-3\theta},\qquad b(0)=0.}
$$

To check that this is an [Bayesian Nash equilibrium](../../../../../bayesian-nash-equilibrium.md) rather than just a necessary formula, its derivative is $b'(\theta)=2(1-\theta)(3-\theta)/[3(2-\theta)^2]$, positive for $0\leq\theta<1$. A type $\theta$ mimicking a type $z$ receives utility $\theta G(z)-m(z)$, whose derivative in $z$ is $(\theta-z)G'(z)$. It is positive before $z=\theta$ and negative after it, so the truthful type-matching bid is globally optimal. Bids above the highest [Bayesian Nash equilibrium](../../../../../bayesian-nash-equilibrium.md) bid can only increase payment without increasing the winning probability; the usual nonnegative bid range covers the lower boundary.

By symmetry and the [law of total expectation](../../../../../law-of-total-expectation.md), **the seller's expected two-item revenue is**

$$
\boxed{R_2=3\int_0^1m(\theta)d\theta=3\left(\frac13-\frac16\right)=\frac12.}
$$

For one item and the same three bidders,

$$
\boxed{R_1=3\int_0^1\frac23\theta^3d\theta=\frac12=R_2.}
$$

More generally the single-item revenue with $n$ bidders is $(n-1)/(n+1)$. Allocating a second item lowers competition enough that it adds no expected revenue in this particular three-bidder uniform model.

The final mechanism is a **[direct revelation mechanism](../../../../../direct-revelation-mechanism.md)** because the message submitted by bidder $i$ is its valuation report, in the same type space $[0,1]$, and allocation and payment are explicit functions of those reports. It is the [Clarke pivot mechanism](../../../../../vickrey-clarke-groves-mechanism.md) for selecting two unit-demand winners. Truthful reporting is a [dominant strategy](../../../../../dominant-strategy.md): bidder $i$'s utility equals its true allocation value plus the other bidders' reported allocation values, minus a term depending only on the others' reports. Reporting its true value makes the efficient allocation maximize the first two terms, while the last is unaffected by its report.

Let the ordered values be $\theta_{(1)}\leq\theta_{(2)}\leq\theta_{(3)}$. For a winner $i$, the maximum welfare achievable by the other two bidders is their combined value; in the actual allocation only the other winner receives an item. Thus the difference defining its payment is the excluded bidder's value $\theta_{(1)}$. For the loser, both other bidders receive items already, so its payment is zero. Consequently **both winners pay the lowest valuation**, and

$$
\boxed{R_{\mathrm{pivot}}=2\,\mathbb E\theta_{(1)}=2\int_0^1\mathbb P(\theta_{(1)}>t)dt=2\int_0^1(1-t)^3dt=\frac12.}
$$

This equals the [first-price sealed-bid auction](../../../../../first-price-sealed-bid-auction.md) revenue above. A conditional check gives the same [interim payment identity](../../../../../interim-payment-identity.md): the minimum of the other two values has density $2(1-z)$, and bidder $i$ wins exactly when that minimum is below $\theta$. Its conditional expected pivot payment is $\int_0^\theta 2z(1-z)dz=\theta^2-2\theta^3/3=m(\theta)$. The mechanisms have equal expected revenue, even though their realized payments need not coincide.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 212](../../paper-212-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
