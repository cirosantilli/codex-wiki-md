<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Rudolph measure rigidity theorem](../../../../../rudolph-measure-rigidity-theorem.md) has an essential ergodicity hypothesis. If a Borel probability measure $\mu$ on the [circle group](../../../../../circle-group.md) is invariant under both $T_2$ and $T_3$, is ergodic for the semigroup generated jointly by these maps, and either map has positive [Kolmogorov-Sinai entropy](../../../../../kolmogorov-sinai-entropy.md), then

$$
\boxed{\mu=m.}
$$

Equivalently, a jointly ergodic common invariant measure other than [Lebesgue measure](../../../../../lebesgue-measure.md) has zero entropy for both maps. Joint ergodicity means that every set invariant modulo $\mu$ under both maps has measure zero or one. Positive entropy without this hypothesis is insufficient: $\tfrac12m+\tfrac12\delta_0$, with $\delta_0$ a [Dirac measure](../../../../../dirac-measure.md), is a common invariant measure of positive entropy and is not $m$.

The [Host equidistribution theorem](../../../../../host-equidistribution-theorem.md) states that if $p,q\geq2$ are relatively prime integers and $\nu$ is invariant and ergodic under $T_p$, with $h_\nu(T_p)>0$, then for $\nu$-almost every $x$ the sequence $(T_q^nx)$ is an [equidistributed sequence](../../../../../equidistributed-sequence.md) for [Lebesgue measure](../../../../../lebesgue-measure.md). Explicitly, for every continuous $g$ on the circle,

$$
\boxed{\frac1N\sum_{n=0}^{N-1}g(T_q^nx)\longrightarrow\int g\,dm
\quad\text{for }\nu\text{-almost every }x.}
$$

The non-ergodic form assumes $T_p$ invariance and positive entropy for almost every component in the [ergodic decomposition](../../../../../ergodic-decomposition.md) $\nu=\int\nu_\omega\,d\lambda(\omega)$. Applying the ergodic theorem of Host on each such component gives the same almost-everywhere conclusion for $\nu$. More generally, its conclusion holds on the part supported on positive-entropy components. A positive value of $h_\nu(T_p)$ alone does not eliminate zero-entropy components.

To deduce the joint version of the [Rudolph measure rigidity theorem](../../../../../rudolph-measure-rigidity-theorem.md), suppose $h_\mu(T_2)>0$; if only $T_3$ has positive entropy, interchange the roles. Write the $T_2$ [ergodic decomposition](../../../../../ergodic-decomposition.md) as $\mu=\int\nu\,d\tau(\nu)$. Since $T_3$ commutes with $T_2$, its [pushforward measure](../../../../../pushforward-measure.md) sends a $T_2$ ergodic component $\nu$ to a $T_2$ ergodic component $(T_3)_*\nu$. On each component, $T_3$ is a [factor of a measure-preserving system](../../../../../factor-of-a-measure-preserving-system.md) with fibres of size at most three. We use the standard [entropy preservation under a finite-to-one factor](../../../../../entropy-preservation-under-a-finite-to-one-factor.md):

$$
h_{(T_3)_*\nu}(T_2)=h_\nu(T_2).
$$

The reason for this standard entropy fact is that, conditional on a complete factor point, every finite orbit name has at most three possibilities; its conditional entropy is bounded by $\log3$, and division by the orbit length gives zero relative entropy.

The component at $T_3x$ is $(T_3)_*\nu_x$ [almost everywhere](../../../../../almost-everywhere.md); this follows from commutation and the componentwise ergodic averages. The component entropy function $r(x)=h_{\nu_x}(T_2)$ is therefore invariant under both $T_2$ and $T_3$. Joint ergodicity makes it constant [almost everywhere](../../../../../almost-everywhere.md), and [affinity of entropy under ergodic decomposition](../../../../../affinity-of-entropy-under-ergodic-decomposition.md) identifies the constant as $h_\mu(T_2)>0$. Thus almost every $T_2$ component has positive entropy, exactly the condition required in the non-ergodic [Host equidistribution theorem](../../../../../host-equidistribution-theorem.md). It follows that $\mu$-almost every point equidistributes for $m$ under $T_3$.

For any continuous $g$, invariance under $T_3$ and the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) now give

$$
\int g\,d\mu
=\int\frac1N\sum_{n=0}^{N-1}g(T_3^nx)\,d\mu(x)
\longrightarrow\int g\,dm.
$$

Continuous functions determine Borel probability measures on the circle, so $\mu=m$, proving the deduction.

For the normal-number example, let $\omega_1,\omega_2,\ldots$ be independent fair binary digits and define

$$
\pi(\omega)=\sum_{j=1}^\infty\frac{2\omega_j}{3^j},\qquad
\nu=\pi_*\left(\left(\tfrac12,\tfrac12\right)^{\mathbb N}\right).
$$

This [Cantor Bernoulli measure](../../../../../cantor-bernoulli-measure.md) is supported on the middle-third [Cantor set](../../../../../cantor-set.md) $C$. If $S$ is the [Bernoulli shift](../../../../../bernoulli-shift.md), then $T_3\circ\pi=\pi\circ S$ on the circle. Consequently $\nu$ is $T_3$ invariant and ergodic: a $T_3$ invariant event pulls back to an $S$ invariant event, which has probability zero or one.

Take the ternary digit [measurable partition](../../../../../measurable-partition.md) $\eta=\{[0,1/3),[1/3,2/3),[2/3,1)\}$. Its block partition of length $n$ has, up to null endpoints, $2^n$ positive-measure atoms under $\nu$, each of measure $2^{-n}$, and all other atoms have measure zero. Hence

$$
H_\nu(\eta_0^{n-1})=n\log2,\qquad
h_\nu(T_3)\geq h_\nu(T_3,\eta)=\log2>0.
$$

Apply the [Host equidistribution theorem](../../../../../host-equidistribution-theorem.md) with $p=3$, $q=2$. For $\nu$-almost every $x\in C$, the sequence $(T_2^nx)$ equidistributes for [Lebesgue measure](../../../../../lebesgue-measure.md), so $x$ is a [normal number](../../../../../normal-number.md) in base $2$ by [normality and equidistribution under integer multiplication](../../../../../normality-and-equidistribution-under-integer-multiplication.md).

The ternary expansion of $\nu$-almost every such $x$ contains only $0$ and $2$, so the frequency of digit $1$ is zero rather than $1/3$. The ambiguous ternary endpoints form a countable $\nu$ null set and can be removed. Therefore $x$ is not a [normal number](../../../../../normal-number.md) in base $3$. We have proved the stronger almost-everywhere existence statement

$$
\boxed{\nu\{x\in C\cap[0,1):x\text{ is normal in base }2\text{ and not normal in base }3\}=1.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 108](../../paper-108-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
