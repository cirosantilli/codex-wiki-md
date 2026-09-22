<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We use [dyadic quadratic variation of Brownian motion](../../../../../../dyadic-quadratic-variation-of-brownian-motion.md). For fixed rational $0\le u<v$, set $\ell=v-u$ and let $Q_n$ be the sum of the squares of the $2^n$ [Brownian increments](../../../../../../brownian-increment.md) on its equal-length partition. [Independence](../../../../../../independent-random-variables.md) and the [normal](../../../../../../normal-distribution.md) [fourth moment](../../../../../../fourth-moment.md) give

$$
\mathbb EQ_n=\ell,\qquad \operatorname{Var}(Q_n)=2\ell^2\,2^{-n}.
$$

For every $\eta>0$, [Chebyshev's inequality](../../../../../../chebyshev-inequality.md) bounds $\mathbb P(|Q_n-\ell|>\eta)$ by $2\ell^2\eta^{-2}2^{-n}$, a summable sequence. The [Borel-Cantelli lemma](../../../../../../borel-cantelli-lemmas.md) implies $Q_n\to\ell$ almost surely. Intersect over positive rational $\eta$ and all rational intervals to obtain one probability-one event on which every such interval has this positive quadratic-variation limit.

If a path were Hölder of exponent $\alpha>1/2$ on a nonempty open interval, choose a compact rational subinterval $[u,v]$ within it and a finite Hölder constant $C$ there. Every partition increment would have absolute value at most $C(\ell2^{-n})^\alpha$, so

$$
Q_n\le C^2\ell^{2\alpha}2^{n(1-2\alpha)}\longrightarrow0.
$$

This contradicts $Q_n\to\ell>0$. The same pathwise event excludes every exponent greater than $1/2$, without needing an uncountable intersection of events. Therefore

$$
\boxed{\text{Almost surely, no nonempty interval supports a Hölder exponent }>\tfrac12.}
$$

This is the [quadratic variation obstruction to Hölder regularity](../../../../../../quadratic-variation-obstruction-to-holder-regularity.md). It rules out a continuously differentiable trajectory on any interval, since a continuous derivative is bounded on smaller compact intervals and gives a [Lipschitz](../../../../../../lipschitz-continuity.md) bound. By itself it does not rule out differentiability at an isolated point. The stronger [nowhere differentiability of Brownian motion](../../../../../../nowhere-differentiability-of-brownian-motion.md) can also be seen directly as follows.

On a mesh of width $h=2^{-n}$ in $[0,M]$, the probability that any specified three consecutive increments all have absolute value at most $Kh$ is at most $C K^3h^{3/2}$: each increment is $N(0,h)$ and the three are [independent](../../../../../../independent-random-variables.md). There are at most $M/h$ possible blocks, so the probability of any such block is at most $C M K^3h^{1/2}$, summable in $n$. By [Borel-Cantelli lemma](../../../../../../borel-cantelli-lemmas.md), for every pair of positive integers $M,K$ there are eventually no such blocks. But a finite derivative at some time $t<M$ would imply $|B_s-B_t|\le C_t|s-t|$ near $t$. The three mesh increments beginning at the mesh point immediately to the left of $t$ would then all be at most $6C_th$ for all sufficiently fine meshes. Choosing an integer $K\ge6C_t$ contradicts the preceding event. Thus finite derivatives do not exist anywhere almost surely, including a finite right derivative at $0$. The Hölder estimates below $1/2$ express continuity with a roughness scale; they do not imply differentiability.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
