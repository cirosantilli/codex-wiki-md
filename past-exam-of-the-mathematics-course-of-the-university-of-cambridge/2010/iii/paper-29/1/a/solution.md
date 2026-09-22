<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set $h_n=2^{-n}$ and $t_n=h_n\lceil t/h_n\rceil$. Replace the last sampled value $X_{t_n}$ by $X_t$, and call the resulting absolute-increment sum $W_n(t)$. This is a sum over a genuine [partition of an interval](../../../../../../partition-of-an-interval.md) of $[0,t]$, and

$$
|V_t^{n,|\cdot|}-W_n(t)|\le |X_{t_n}-X_t|\longrightarrow0
$$

by right continuity. This is the [dyadic approximation of total variation](../../../../../../dyadic-approximation-of-total-variation.md). Let $V(t)$ be the [total variation of a function](../../../../../../total-variation-of-a-function.md) $X$ on $[0,t]$, allowing $+\infty$. Every $W_n(t)$ is at most $V(t)$. Conversely, take any finite [partition of an interval](../../../../../../partition-of-an-interval.md) of $[0,t]$. Approximate its interior points from the right by dyadic grid points, retaining the endpoint $t$. For large $n$ these approximating points remain distinct, and right continuity makes their absolute-increment sum converge to that of the original partition. The [triangle inequality](../../../../../../triangle-inequality.md) makes $W_n(t)$ at least this selected sum. Taking the [supremum](../../../../../../supremum.md) over all partitions proves

$$
\boxed{\lim_{n\to\infty}V_t^{n,|\cdot|}=V(t),\quad V(t)=\operatorname{Var}_{[0,t]}X\in[0,\infty].}
$$

The limit is the total-variation function; for locally finite variation it is the [total-variation process](../../../../../../total-variation-process.md).

There is a missing hypothesis in the assertion about being [càdlàg](../../../../../../cadlag.md). A general [càdlàg function](../../../../../../cadlag.md) can have infinite [total variation of a function](../../../../../../total-variation-of-a-function.md) arbitrarily close to zero. For example,

$$
X_0=0,\qquad X_s=s\sin(1/s)\quad(s>0)
$$

is continuous. At the successive points $s_j=(\pi/2+j\pi)^{-1}$ its values alternate in sign with magnitude $s_j$. The variation along these points dominates a divergent harmonic series. Thus $V(t)=\infty$ for every $t>0$, but $V(0)=0$, so even extended-valued right continuity fails at zero.

The correct [càdlàg](../../../../../../cadlag.md) conclusion holds when $X$ has [finite variation](../../../../../../total-variation-of-a-function.md) on every compact interval. Indeed $V$ is then finite and nondecreasing, so it has finite left limits. To prove right continuity at $t$, fix $s>t$ and choose a partition of $[t,s]$ whose sum is within $\varepsilon$ of its variation. If $u>t$ lies before the first interior partition point, changing the first endpoint from $t$ to $u$ changes that sum by at most $|X_u-X_t|$. Additivity of [total variation of a function](../../../../../../total-variation-of-a-function.md) therefore gives

$$
0\le V(u)-V(t)\le\varepsilon+|X_u-X_t|.
$$

Let $u\downarrow t$ and then $\varepsilon\downarrow0$. This proves right continuity. This proves [càdlàg regularity of finite total variation](../../../../../../cadlag-regularity-of-finite-total-variation.md). Under that qualification, the jump formula is

$$
\boxed{\Delta V_t=|\Delta X_t|=|X_t-X_{t-}|\qquad(t>0).}
$$

If the variation is infinite, a difference of two infinite variation values is not a defined jump.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
