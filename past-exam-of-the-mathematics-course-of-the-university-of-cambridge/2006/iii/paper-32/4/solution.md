<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For standard [Brownian motion](../../../../../brownian-motion-split.md) $B$ and $h>0$, let $T_h$ be its first hitting time of $h$. Define the reflected path by

$$
\widehat B_t=\begin{cases}B_t,&t\leq T_h,\\2h-B_t,&t>T_h,\end{cases}
$$

leaving a path unchanged if $T_h=\infty$. The **[Brownian reflection principle](../../../../../reflection-principle-wiener-process.md)** says that $\widehat B$ has the same path [probability distribution](../../../../../probability-distribution.md) as $B$. In its endpoint form, for $t>0$ and every Borel set $A\subset(-\infty,h)$,

$$
\mathbb P(T_h\leq t,\ B_t\in A)=\mathbb P(B_t\in2h-A),
\qquad 2h-A=\{2h-y:y\in A\}.
$$

Here is a direct proof of preservation of the path law. For a fixed integer horizon $L$, let $T^{(m)}=2^{-m}\lceil2^mT_h\rceil\wedge L$, with an infinite first term interpreted as infinity. This is a [stopping time](../../../../../stopping-time.md) taking finitely many deterministic grid values. On $\{T^{(m)}=j2^{-m}\}$, the history determining that event is measurable at $j2^{-m}$, and subsequent [Brownian motion](../../../../../brownian-motion-split.md) increments are independent of that history. Those increments and their negatives have the same joint law, by symmetry of centered [normal distributions](../../../../../normal-distribution.md) and [independent increments](../../../../../independent-increments.md). Thus reflecting after $T^{(m)}$ around $B_{T^{(m)}}$ preserves the full path law. For any fixed horizon $t<L$, the reflected paths converge uniformly on $[0,t]$ to the displayed reflected path, by [continuity](../../../../../continuous-function.md) as $T^{(m)}$ decreases to $T_h\wedge L$. This includes $T_h=\infty$, since reflection after $L$ has no effect before $t$. Passing to all finite-dimensional [probability distributions](../../../../../probability-distribution.md) proves the assertion; no prior recurrence claim is needed. Equivalently, the [Strong Markov property](../../../../../strong-markov-property.md) gives the same proof by symmetry of the fresh increments after the hit. Reflection is an involution preserving the hitting event and mapping the indicated endpoint $y$ to $2h-y$. An endpoint above $h$ forces a hit by [continuity](../../../../../continuous-function.md); this proves the endpoint identity, rather than assuming it.

For $S_t=\sup_{0\leq s\leq t}B_s$, split $\{T_h\leq t\}$ according to whether $B_t$ is above or below $h$. Since $B_t$ has no atom at $h$, reflection gives

$$
\mathbb P(S_t\geq h)=\mathbb P(B_t\geq h)+\mathbb P(T_h\leq t,\ B_t<h)
=2\mathbb P(B_t\geq h)=\mathbb P(|B_t|\geq h).
$$

Both variables are nonnegative, so their positive tails identify the law:

$$
\boxed{S_t\stackrel d=|B_t|.}
$$

For $t>0$ this is the [half-normal distribution](../../../../../half-normal-distribution.md) of scale $\sqrt t$; at $t=0$ both variables vanish.

For the two separated intervals, put

$$
A_0=\sup_{a\leq t\leq b}B_t-B_b,\qquad Z=B_c-B_b,\qquad H=\sup_{0\leq u\leq d-c}(B_{c+u}-B_c).
$$

Here $A_0$ is measurable for $\mathcal F_b$, $Z$ has the [normal distribution](../../../../../normal-distribution.md) $N(0,c-b)$, and $H$ is a function of increments after $c$. The [independent increments](../../../../../independent-increments.md) make these three objects mutually independent. The later absolute maximum is $B_b+Z+H$, so equality of the two maxima means $Z=A_0-H$. Conditional on $(A_0,H)$, this specifies a single value of the nondegenerate [normal distribution](../../../../../normal-distribution.md) $Z$, and hence has probability zero. Therefore

$$
\boxed{\mathbb P\left(\sup_{a\leq t\leq b}B_t=\sup_{c\leq t\leq d}B_t\right)=0.}
$$

This proves the [atomless maxima on separated Brownian intervals](../../../../../atomless-maxima-on-separated-brownian-intervals.md) without incorrectly treating the two absolute maxima as independent.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
