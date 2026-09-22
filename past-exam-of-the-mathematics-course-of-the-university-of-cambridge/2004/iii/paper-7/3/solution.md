<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

We first construct a terminal integrable function without using the [martingale convergence theorem](../../../../../martingale-convergence-theorem.md). Put $G=\sup_n|g_n|$ and $d\eta=G\,dx$ on $(0,1]^d$. This is a finite positive measure. If $G=0$ almost everywhere the conclusion is immediate. Otherwise, for a bounded dyadic step function $h$ measurable with respect to $\mathcal F_n$ in the [dyadic filtration](../../../../../dyadic-filtration.md), define

$$
\Lambda(h)=\int h g_n\,dx.
$$

The [martingale](../../../../../martingale-split.md) property makes the definition independent of the choice of a sufficiently large $n$. Moreover $|\Lambda(h)|\leq\int|h|\,d\eta$. Dyadic step functions are dense in $L^1(\eta)$: [continuous functions](../../../../../continuous-function.md) on the closed unit cube are dense for this finite [Borel measure](../../../../../borel-measure.md) (extend the measure by zero onto the omitted faces), and [uniform continuity](../../../../../uniform-continuity.md) approximates each [continuous function](../../../../../continuous-function.md) by step functions on fine dyadic partitions. Thus $\Lambda$ extends to a [bounded linear functional](../../../../../continuous-linear-functional.md) on $L^1(\eta)$ of [norm](../../../../../norm.md) at most one. The [duality of Lp spaces](../../../../../duality-of-lp-spaces.md) representation of this functional gives $H\in L^\infty(\eta)$ with $|H|\leq1$ and $\Lambda(h)=\int hH\,d\eta$. Set $g=HG$, taking $g=0$ where $G=0$. Then $g\in L^1(dx)$ and testing indicators of all dyadic atoms proves

$$
\boxed{g_n=\mathbb E(g\mid\mathcal F_n).}
$$

This argument also works for complex-valued [martingales](../../../../../martingale-split.md), with a complex [linear functional](../../../../../linear-functional.md).

To prove convergence, choose a dyadic step function $h$ with $\|g-h\|_1$ arbitrarily small. For all $n$ beyond its dyadic level, $\mathbb E(h\mid\mathcal F_n)=h$. The [L1 contraction of conditional expectation](../../../../../l1-contraction-of-conditional-expectation.md) yields

$$
\|g_n-g\|_1\leq\|\mathbb E(g-h\mid\mathcal F_n)\|_1+\|g-h\|_1
\leq2\|g-h\|_1.
$$

This proves convergence in $L^1$. For convergence [almost everywhere](../../../../../almost-everywhere.md), [Doob maximal inequality](../../../../../doob-maximal-inequality-for-a-nonnegative-submartingale.md) applied to the [conditional expectations](../../../../../conditional-expectation.md) of $g-h$ gives

$$
\begin{aligned}
\left|\left\{\limsup_n|g_n-g|>2a\right\}\right|
&\leq\left|\left\{\sup_n|\mathbb E(g-h\mid\mathcal F_n)|>a\right\}\right|
+|\{|g-h|>a\}|\\
&\leq\frac{2\|g-h\|_1}{a}.
\end{aligned}
$$

Let the approximation error tend to zero, and then take positive rational $a$. Hence **$g_n\to g$ both in $L^1$ and almost everywhere**.

For the second assertion, write $M=\sup_n\mathbb E|f_n|<\infty$ and take the given first-exit [stopping time](../../../../../stopping-time.md) $\tau$. Each $g_n=f_{\tau\wedge n}$ is integrable, being a finite sum of restrictions of integrable variables. Its increments satisfy

$$
g_{n+1}-g_n=\mathbf1_{\{\tau>n\}}(f_{n+1}-f_n).
$$

The indicator is $\mathcal F_n$-measurable, so taking its [conditional expectation](../../../../../conditional-expectation.md) proves that $(g_n)$ is a [martingale](../../../../../martingale-split.md).

The overshoot at $\tau$ need not be bounded by $N$. Instead, for a fixed $m$, on $\{\tau=j\}$ with $j\leq m$ we have $|f_j|\leq\mathbb E(|f_m|\mid\mathcal F_j)$. Integrating over this $\mathcal F_j$-measurable event, summing the disjoint events, and including $\{\tau>m\}$ gives

$$
\mathbb E|g_m|\leq\mathbb E|f_m|\leq M.
$$

The variables $Z_m=|f_\tau|\mathbf1_{\{\tau\leq m\}}$ increase to $Z$, and $Z_m\leq|g_m|$. The [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) gives $\mathbb E Z\leq M$. Before stopping, the process has magnitude less than $N$; after stopping it remains at $f_\tau$. Consequently

$$
\boxed{g^*\leq Z\vee N,\qquad\mathbb E(Z\vee N)\leq M+N<\infty.}
$$

This is the [integrable overshoot of a stopped L1-bounded martingale](../../../../../integrable-overshoot-of-a-stopped-l1-bounded-martingale.md). The first part now proves that every such stopped process converges [almost everywhere](../../../../../almost-everywhere.md).

Finally, [Doob maximal inequality](../../../../../doob-maximal-inequality-for-a-nonnegative-submartingale.md) gives $|\{\sup_n|f_n|\geq N\}|\leq M/N$, by applying the finite-horizon estimate and then increasing the horizon. Thus $\sup_n|f_n|$ is finite [almost everywhere](../../../../../almost-everywhere.md). Outside the union of the null sets for all positive integer stopping thresholds, choose an integer $N$ larger than this supremum. No stopping occurs at that point, so $f_n=g_n$ for all $n$, and **$f_n$ converges to a finite limit almost everywhere**. We have not assumed, or concluded, $L^1$ convergence for this general $L^1$-bounded [martingale](../../../../../martingale-split.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
