<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $\mu=Du$, a finite signed [Radon measure](../../../../../../radon-measure.md), and define

$$
F_l(t)=\mu((a,t)),\qquad F_r(t)=\mu((a,t]).
$$

For $\varphi\in C_c^1((a,b))$, [Fubini's theorem](../../../../../../fubini-s-theorem.md) for the [signed measure](../../../../../../signed-measure.md) gives

$$
-\int_a^bF_l(t)\varphi'(t)dt=-\int_{(a,b)}\!\left[\int_s^b\varphi'(t)dt\right]d\mu(s)=\int\varphi\,d\mu.
$$

Thus $DF_l=\mu=Du$. A distribution on a connected interval with zero [derivative](../../../../../../derivative.md) is constant: any compactly supported test of integral zero is the [derivative](../../../../../../derivative.md) of a compactly supported test, so it pairs to zero with $u-F_l$. Choose the resulting constant $c$. Then

$$
\boxed{u_l(t)=c+\mu((a,t)),\qquad u_r(t)=c+\mu((a,t])}
$$

are [one-sided representatives of a one-dimensional BV function](../../../../../../one-sided-representatives-of-a-one-dimensional-bv-function.md). The first equals $u$ [almost everywhere](../../../../../../almost-everywhere.md). Their difference is $\mu(\{t\})$, nonzero at at most countably many points, so the second also equals $u$ [almost everywhere](../../../../../../almost-everywhere.md).

Finite-measure continuity applied to $|\mu|$ proves $F_l(s)\to F_l(t)$ as $s\uparrow t$, and $F_r(s)\to F_r(t)$ as $s\downarrow t$. Moreover the opposite one-sided limits are $F_l(t+)=F_r(t)$ and $F_r(t-)=F_l(t)$. Consequently both representatives are continuous exactly where $\mu(\{t\})=0$. For each positive integer $m$, there are only finitely many [measure atoms](../../../../../../atom-measure-theory.md) of magnitude at least $1/m$, since their total magnitudes are bounded by $|\mu|((a,b))$. Their union is countable, proving the requested discontinuity bound. This does not require the jump points to be isolated; they can be dense.

The hint's one-dimensional statement is consistent with this construction: zero $\mathcal H^0$ [measure](../../../../../../measure.md) means an empty set, so $S_u\subseteq J_u$. This concerns approximate discontinuities of the [BV space](../../../../../../function-of-bounded-variation-on-a-domain.md) class; arbitrary changes of representative at points could create artificial pointwise discontinuities. The interval-mass representatives above remove that ambiguity and give the required one-sided continuity directly.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
