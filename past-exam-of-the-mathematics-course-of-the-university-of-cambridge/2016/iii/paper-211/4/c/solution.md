<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $b$ and $h$ be the numbers of units of the [numéraire](../../../../../../numeraire.md) and the [stock](../../../../../../stock.md) in a [replicating strategy](../../../../../../replicating-strategy.md). The two terminal payoffs of the [European call option](../../../../../../european-call-option.md) are $2$ and $0$, so

$$
15b+20h=2,\qquad20b+15h=0.
$$

Solving these simultaneous equations gives $b=-6/35$ and $h=8/35$. **The initial replication cost is**

$$
\boxed{C(1,18)=10b+10h=\frac47.}
$$

As an independent pricing check, let $q$ be the [risk-neutral probability](../../../../../../risk-neutral-probability.md) of the state $(15,20)$ under the [numéraire](../../../../../../numeraire.md) measure. The discounted [stock](../../../../../../stock.md) must have initial value one and terminal mean one:

$$
1=q\frac{20}{15}+(1-q)\frac{15}{20},\qquad q=\frac37.
$$

[Risk-neutral valuation](../../../../../../risk-neutral-pricing.md) then gives $10(3/7)(2/15)=4/7$. The physical probabilities $1/2,1/2$ are not the [numéraire](../../../../../../numeraire.md)-measure probabilities.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
