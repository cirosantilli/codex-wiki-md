<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under the path convention used here, a real [Lévy process](../../../../../../levy-process.md) $(L_a)_{a\geq0}$ starts at zero, has [independent increments](../../../../../../independent-increments.md) and [stationary increments](../../../../../../stationary-increments.md), is [stochastically continuous](../../../../../../stochastic-continuity.md), and has [càdlàg](../../../../../../cadlag.md) paths almost surely. We verify all four requirements for $S$.

The immediate positive excursions proved in part (b) give $S_0=0$. For a deterministic $a\geq0$, $S_a$ is an almost-surely finite [stopping time](../../../../../../stopping-time.md), and continuity gives $X_{S_a}=a$. The [Strong Markov property](../../../../../../strong-markov-property.md) implies that $\widetilde X_t=X_{S_a+t}-a$ is a fresh Brownian motion independent of the information up to $S_a$. For $b\geq0$,

$$
S_{a+b}-S_a=\inf\{t\geq0:\widetilde X_t>b\}.
$$

No crossing of $a+b$ could have occurred before $S_a$. The increment thus has the same law as $S_b$ and is independent of the past. Apply this successively at a finite increasing sequence of deterministic levels to prove stationary independent increments.

For $h>0$ and $\varepsilon>0$, part (b) and reflection give

$$
\mathbb P(S_h>\varepsilon)=2\Phi(h/\sqrt\varepsilon)-1\longrightarrow0
\quad(h\downarrow0).
$$

Hence $S_h\to0$ in probability. Stationarity of the increments gives stochastic continuity at every level, from either side where defined.

For path regularity, on a single probability-one event the [Brownian running maximum](../../../../../../brownian-running-maximum.md) $M_t=\max_{s\leq t}X_s$ is continuous, nondecreasing and unbounded, and

$$
S_a=\inf\{t:M_t>a\}.
$$

This inverse is nondecreasing. If $a_j\downarrow a$, then $S_{a_j}\downarrow L\geq S_a$. For any $t>S_a$, some $u<t$ has $M_u>a$; for all sufficiently large $j$, $M_u>a_j$, so $S_{a_j}\leq u<t$. Thus $L=S_a$, proving right continuity at every level simultaneously. On each bounded level interval it is bounded by the finite value at a larger integer level. Monotonicity then gives finite left limits. Therefore

$$
\boxed{S\text{ is a càdlàg Lévy process, the Brownian first-passage subordinator}.}
$$

The [Brownian first-passage subordinator](../../../../../../brownian-first-passage-subordinator.md) is the level-indexed increasing process, rather than a process indexed by the original Brownian time.

For $H$, the inverse relations for a continuous running maximum are

$$
H_a=S_{a-}\quad(a>0),\qquad H_{a+}=S_a.
$$

For example, if $b<a$ then $S_b\leq H_a$; while for $t<H_a$, $M_t<a$ and any $b\in(M_t,a)$ has $S_b>t$. Taking limits gives $S_{a-}=H_a$. Similarly $H_b\geq S_a$ for $b>a$, and a crossing of any level strictly above $a$ before a given $t>S_a$ bounds $H_b$ from above for $b$ sufficiently close to $a$. This proves $H_{a+}=S_a$. These are the [non-strict inverse of a continuous nondecreasing function](../../../../../../non-strict-inverse-of-a-continuous-nondecreasing-function.md) identities.

At the random level $A$ in part (b), $H_A<S_A=H_{A+}$, so $H$ fails right continuity almost surely. Thus it is not a [Lévy process](../../../../../../levy-process.md) under the stated càdlàg-path convention. It does have the same [finite-dimensional distributions](../../../../../../finite-dimensional-distribution.md) and stochastic continuity as $S$, so definitions of a Lévy process that require only the increment and stochastic-continuity properties would call $H$ a Lévy process with a càdlàg modification. The reason for excluding the particular version $H$ here is its path regularity.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
