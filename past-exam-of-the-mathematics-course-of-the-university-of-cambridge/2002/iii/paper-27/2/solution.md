<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In discrete time, the bounded-time [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) says that an integrable [supermartingale](../../../../../supermartingale.md) $X$ and bounded [stopping times](../../../../../stopping-time.md) $S\le T$ satisfy $\mathbb E[X_T\mid\mathcal F_S]\le X_S$. For a [martingale](../../../../../martingale-split.md) there is equality. The assertion at a possibly unbounded, almost-surely finite [stopping time](../../../../../stopping-time.md) $T$ also holds with $S=0$ if $\{X_{T\wedge n}:n\ge0\}$ is [uniformly integrable](../../../../../uniform-integrability.md): then $X_T$ is integrable and $\mathbb EX_T\le\mathbb EX_0$, with equality for a [martingale](../../../../../martingale-split.md). Boundedness of $T$ or the stated integrability condition cannot in general be omitted.

For the increment hypothesis here, $\mathbb ET<\infty$ implies $T<\infty$ almost surely, and telescoping gives

$$
|X_{T\wedge n}|\le|X_0|+KT,\qquad |X_T|\le|X_0|+KT.
$$

The right-hand side is an [integrable random variable](../../../../../integrable-random-variable.md). Applying bounded-time [optional stopping](../../../../../optional-sampling-theorem-for-a-supermartingale.md) to $T\wedge n$ and then the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) proves

$$
\boxed{X_T\in L^1,\qquad \mathbb EX_T\le\mathbb EX_0.}
$$

This is [bounded-increment optional stopping with integrable time](../../../../../bounded-increment-optional-stopping-with-integrable-time.md); the same reasoning gives equality for a [martingale](../../../../../martingale-split.md).

Put $q=1-p$ and first assume $0<p<1$. Let $\tau$ be the first occurrence time of the specified seven-letter word. Its probability in a prescribed block is $r=p^4q^3>0$. Disjoint seven-flip blocks are [independent](../../../../../independent-random-variables.md), and a match in one forces $\tau$ to have occurred by its end. Consequently $\mathbb P(\tau>7m)\le(1-r)^m$ and $\mathbb E\tau\le7/r<\infty$; this establishes the integrability needed for stopping before computing its value.

Start a new gambler with unit capital immediately before each flip. A gambler bets all current capital on the next required letter of the word, receives capital divided by $p$ for a correct head or by $q$ for a correct tail, and receives zero on failure. After completing all seven bets, the gambler retains the winnings without further betting. Each individual bet preserves its conditional expected capital. If $C_n$ is the total capital of all gamblers who have entered through flip $n$, then $C_n-n$ is a [martingale](../../../../../martingale-split.md).

At any time at most seven gamblers are still betting, and each one's capital is at most $L=1/(p^4q^3)$, since probabilities of shorter prefixes are at least the full-word probability. Completed winnings do not change. Thus the increments of $C_n-n$ have a deterministic bound, for example $14L+1$. The preceding optional-stopping argument therefore gives $\mathbb E(C_\tau-\tau)=0$.

At the first full match, no earlier gambler has completed the word. A surviving gambler who has placed $k$ successful bets corresponds to a suffix of the completed word which is also its length-$k$ prefix, namely a [border of a word](../../../../../border-of-a-word.md). The only such lengths are $3$ and $7$: the shorter common string is HHT. Their capitals are $1/(p^2q)$ and $1/(p^4q^3)$, respectively. Hence $C_\tau$ is this deterministic sum and

$$
\boxed{\mathbb E\tau=\frac1{p^4(1-p)^3}+\frac1{p^2(1-p)}.}
$$

For a fair coin this is **136 flips**. This is a [waiting time for a word in independent nonuniform symbols](../../../../../waiting-time-for-a-word-in-independent-nonuniform-symbols.md); the overlap contribution is essential. If $p=0$ or $p=1$, the word cannot occur because it contains both types of flip, so the expected waiting time is infinite.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
