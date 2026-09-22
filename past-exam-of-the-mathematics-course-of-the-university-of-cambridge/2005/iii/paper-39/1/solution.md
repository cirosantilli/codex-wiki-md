<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Equip $S$ with a sigma-algebra $\mathcal S$. A [Poisson random measure](../../../../../poisson-random-measure.md) with [intensity measure of a point process](../../../../../intensity-measure-of-a-point-process.md) $\mu$ is a random [counting measure](../../../../../counting-measure.md) $\Pi$ such that, for every measurable $A$ with $\mu(A)<\infty$,

$$
\mathbb P(\Pi(A)=k)=e^{-\mu(A)}\frac{\mu(A)^k}{k!},\qquad k=0,1,\ldots,
$$

and the counts on every finite collection of pairwise disjoint measurable sets are independent. Thus $\mathbb E\Pi(A)=\mu(A)$. For a [sigma-finite measure](../../../../../sigma-finite-measure.md) $\mu$, sets of infinite intensity contain infinitely many points almost surely: exhaust such a set by increasing finite-intensity sets and use the Poisson count tails as their means tend to infinity. The count is a measurable [random variable](../../../../../random-variable-split.md) for every measurable $A$, which is part of saying that $\Pi$ is a [random measure](../../../../../random-measure.md).

Under the usual point representation write $\Pi=\sum_j\delta_{Z_j}$, counting multiplicities. If $\mu$ is a [non-atomic measure](../../../../../non-atomic-measure.md), this is a simple [Poisson point process](../../../../../poisson-point-process.md); if $\mu$ has atoms, several point occurrences can have the same location, and each occurrence is counted separately. In a topological setting, local finiteness requires that the intensity be finite on compact sets.

Sufficient existence conditions are that $S$ is a [standard Borel space](../../../../../standard-borel-space.md) and $\mu$ is a [sigma-finite measure](../../../../../sigma-finite-measure.md). This gives [existence of a Poisson random measure on a standard Borel space](../../../../../existence-of-a-poisson-random-measure-on-a-standard-borel-space.md). If a simple locally finite configuration is desired, additionally take a non-atomic, locally finite intensity on a locally compact second-countable Hausdorff space. These conditions are sufficient, not claimed necessary. In particular sigma-finiteness suffices for a countable family of occurrences that can each be independently coloured.

Let $R$ and $G$ be the red and green counting measures. The marking assumption means that, conditional on $\Pi$, the colours of all point occurrences are independent, with the same red [probability](../../../../../probability.md) $r$. For a [measurable set](../../../../../measurable-set.md) $A$ of finite intensity $m=\mu(A)$, condition on its total count. To obtain $a$ red and $b$ green points the total must be $a+b$, so direct multiplication gives the [joint red and green Poisson count formula](../../../../../joint-red-and-green-poisson-count-formula.md)

$$
\begin{aligned}
\mathbb P(R(A)=a,G(A)=b)&=e^{-m}\frac{m^{a+b}}{(a+b)!}\binom{a+b}{a}r^a(1-r)^b\\
&=\left[e^{-rm}\frac{(rm)^a}{a!}\right]\left[e^{-(1-r)m}\frac{((1-r)m)^b}{b!}\right].
\end{aligned}
$$

Thus the two counts are independent Poisson variables with respective means $rm$ and $(1-r)m$. This computation includes zero intensity with the usual convention for the [probability](../../../../../probability.md) of zero counts.

For disjoint finite-intensity sets $A_1,\ldots,A_k$, the original counts are independent. Conditional marking in different sets uses disjoint collections of independent colours. Repeating the preceding calculation therefore gives

$$
\mathbb P\bigl(R(A_i)=a_i,G(A_i)=b_i\text{ for all }i\bigr)=\prod_{i=1}^k\left[e^{-r\mu(A_i)}\frac{(r\mu(A_i))^{a_i}}{a_i!}\right]\prod_{i=1}^k\left[e^{-(1-r)\mu(A_i)}\frac{((1-r)\mu(A_i))^{b_i}}{b_i!}\right].
$$

This proves the disjoint-count definition for each coloured [Poisson point process](../../../../../poisson-point-process.md) and independence of their two count vectors.

To obtain independence of the whole processes, take any finite list of red test sets and any finite list of green test sets, initially all of finite intensity. Refine their union into the disjoint cells given by their membership patterns. Every test-set count is the sum of the counts of its cells. The entire red cell vector is independent of the entire green cell vector by the product formula, hence so are the corresponding test-set count vectors. For arbitrary measurable test sets, intersect first with a finite-intensity exhaustion of $S$ and pass to the increasing count limits. The count cylinder events generate the two evaluation sigma-algebras, and [independence extended from generating pi-systems](../../../../../independence-extended-from-generating-pi-systems.md) gives independence of those sigma-algebras. Consequently

$$
\boxed{R\text{ and }G\text{ are independent Poisson point processes, with intensities }r\mu\text{ and }(1-r)\mu.}
$$

This is a direct count proof of the [Poisson thinning theorem](../../../../../poisson-thinning-theorem.md); no general marking or thinning result has been used to deduce it.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
