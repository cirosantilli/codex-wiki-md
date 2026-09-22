<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

First, [convergence in probability](../../../../../../convergence-in-probability.md) at $t=0$ gives $X_0=0$ [almost surely](../../../../../../almost-sure-convergence.md), since every $X_0^n=0$. For any finite set of times, the corresponding vectors converge in probability: the [union bound](../../../../../../boole-s-inequality.md) controls the probability that any coordinate differs by more than a fixed tolerance. The same holds for their increment vectors, hence also for their [convergence in distribution](../../../../../../convergence-in-distribution.md).

For $0=t_0<t_1<\cdots<t_m$, set $D_j^n=X^n_{t_j}-X^n_{t_{j-1}}$ and $D_j=X_{t_j}-X_{t_{j-1}}$. The [characteristic function of a random vector](../../../../../../characteristic-function-of-a-random-vector.md) factors for the independent increments of each $X^n$:

$$
\mathbb E\exp\left(i\sum_{j=1}^m\theta_jD_j^n\right)=\prod_{j=1}^m\mathbb E e^{i\theta_jD_j^n}.
$$

Pass to the limit using [convergence in distribution](../../../../../../convergence-in-distribution.md) and bounded [continuous functions](../../../../../../continuous-function.md). The resulting factorization of the [characteristic function of a random vector](../../../../../../characteristic-function-of-a-random-vector.md), with the [uniqueness theorem for characteristic functions](../../../../../../uniqueness-theorem-for-characteristic-functions.md), proves [independence](../../../../../../independent-random-variables.md) of the $D_j$. Similarly $X^n_{s+t}-X^n_s\overset d=X^n_t$ passes to the limit, proving [stationary increments](../../../../../../stationary-increments.md) for $X$.

It remains to prove [stochastic continuity](../../../../../../stochastic-continuity.md). For $\varepsilon>0$, the [triangle inequality](../../../../../../triangle-inequality.md) and the [union bound](../../../../../../boole-s-inequality.md) imply, for every fixed $n$,

$$
\begin{aligned}
\limsup_{t\downarrow0}\mathbb P(|X_t|>\varepsilon)
&\leq\limsup_{t\downarrow0}\mathbb P(|X_t-X_t^n|>\varepsilon/2)
+\limsup_{t\downarrow0}\mathbb P(|X_t^n|>\varepsilon/2)\\
&=\limsup_{t\downarrow0}\mathbb P(|X_t-X_t^n|>\varepsilon/2).
\end{aligned}
$$

The second term vanishes by [stochastic continuity](../../../../../../stochastic-continuity.md) of $X^n$. Now let $n\to\infty$ and use the additional near-zero approximation hypothesis. We obtain $X_t\to0$ in probability as $t\downarrow0$. The [stationary increments](../../../../../../stationary-increments.md) transfer this to every time: both $X_{s+h}-X_s$ and $X_s-X_{s-h}$ have the law of $X_h$ for $h>0$ when defined. Thus **$X$ has all the intrinsic [Lévy process](../../../../../../levy-process.md) properties**, proving [closure of Lévy processes under locally controlled convergence in probability](../../../../../../closure-of-levy-processes-under-locally-controlled-convergence-in-probability.md).

If one requires the supplied process itself to be [càdlàg](../../../../../../cadlag.md), the hypotheses justify a [càdlàg modification](../../../../../../cadlag-modification.md), rather than that stronger pathwise assertion. To see the distinction, take $X^n\equiv0$, let $U$ have [uniform distribution](../../../../../../continuous-uniform-distribution.md) on $(0,1)$, and put $X_t=\mathbf1_{\{t=U\}}$. At each fixed time $t$, $X_t=0$ [almost surely](../../../../../../almost-sure-convergence.md), so both approximation hypotheses hold with zero error probability. Nevertheless every path has an isolated spike at $U$ and is not right-continuous there. Its identically zero [modification of a stochastic process](../../../../../../modification-of-a-stochastic-process.md) is a [Lévy process](../../../../../../levy-process.md) with [càdlàg](../../../../../../cadlag.md) paths. **The conclusion is exact under the intrinsic definition, and exact up to modification under the convention requiring [càdlàg](../../../../../../cadlag.md) paths.**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
