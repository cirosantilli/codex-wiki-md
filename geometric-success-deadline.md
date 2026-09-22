# Geometric success deadline

↑ **Parent:** [Geometric distribution](geometric-distribution.md)

How many attempts give at least a chosen success [probability](probability.md) $0<\alpha<1$? For a positive-integer [geometric distribution](geometric-distribution.md) with $0<p<1$, completion by attempt $N$ means $T\leq N$, so

$$
\mathbb P(T\leq N)\geq\alpha
\quad\Longleftrightarrow\quad
q^N\leq1-\alpha
\quad\Longleftrightarrow\quad
N\geq\frac{\log(1-\alpha)}{\log q},\qquad q=1-p.
$$

The [logarithm](logarithm.md) $\log q$ is negative, which reverses the inequality when dividing. The least [integer](integer-split.md) meeting the target is therefore obtained with the [ceiling function](ceiling-function.md):

$$
N_{\alpha}=\left\lceil\frac{\log(1-\alpha)}{\log(1-p)}\right\rceil.
$$

For our constructed [independent](independent-random-variables.md) retry mechanism with $p=0.3$ and $\alpha=0.95$,

$$
\frac{\log(0.05)}{\log(0.7)}\approx8.3991,\qquad N_{0.95}=9.
$$

To verify minimality directly, eight attempts give $\mathbb P(T\leq8)=1-0.7^8=0.94235199<0.95$, whereas nine give $\mathbb P(T\leq9)=1-0.7^9=0.959646393\geq0.95$. Under the zero-based convention, the same completion [event](event.md) is $F\leq8$, with failure to complete given by $F\geq9$; saying $F\leq9$ would allow ten attempts. A 95% deadline controls a tail [probability](probability.md), while the [expected value](expected-value-split.md) $10/3$ describes an average.

At $p=1$ success occurs on the first attempt, so $N_{\alpha}=1$; the [logarithm](logarithm.md) formula is inapplicable. At $p=0$ no finite deadline achieves a positive target. For $0<p<1$, no finite deadline guarantees success with [probability](probability.md) one because $q^N>0$. A retry cap at $N$ produces the [capped geometric waiting time](capped-geometric-waiting-time.md) $\min(T,N)$ as the number of attempts actually spent; reaching the cap can mean either success on the last allowed attempt or failure of all $N$ attempts.

## ↑ Ancestors (8)

1. [Geometric distribution](geometric-distribution.md)
2. [Discrete probability distribution](discrete-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Geometric distribution](geometric-distribution.md)
