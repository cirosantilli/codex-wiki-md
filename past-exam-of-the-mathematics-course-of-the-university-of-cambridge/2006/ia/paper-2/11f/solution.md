<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

After the top card is fixed, precisely three of the remaining fifty-one cards have the same rank. Thus a fresh uniformly shuffled deck has matching probability

$$
\boxed{a=\mathbb P(\text{matching endpoints})=\frac3{51}=\frac1{17}.}
$$

In each independent round, the algorithm repeats with probability $r=(1-a)p=16p/17$ and stops with probability $1-r$. A match always stops. Summing the probabilities over the possible number of repeated rounds gives

$$
\boxed{\mathbb P(X=Y)=\sum_{j=0}^\infty r^ja=\frac1{17-16p}.}
$$

For $0\le p\le1$ the stopping probability per round is at least $1/17$, so termination is almost sure.

Permutation of the thirteen rank labels preserves both the uniform shuffle and the stopping rule. The two [marginal distributions](../../../../../marginal-distribution.md) are consequently uniform:

$$
\boxed{\mathbb P(X=x)=\mathbb P(Y=y)=\frac1{13}\quad(x,y\in\mathcal F).}
$$

To establish [independence](../../../../../independent-random-variables.md), it is necessary to check the [joint probability distribution](../../../../../joint-probability-distribution.md), not just these marginals. For a specified rank $x$, the fresh-shuffle diagonal probability is $(1/13)(3/51)=1/221$. For different specified ranks $x,y$, it is $(1/13)(4/51)=4/663$. Reweight by the acceptance probability and sum over repeated rounds to obtain

$$
\mathbb P(X=x,Y=y)=\begin{cases}
\displaystyle\frac1{13(17-16p)},&x=y,\\
\displaystyle\frac{4(1-p)}{39(17-16p)},&x\ne y.
\end{cases}
$$

The diagonal must equal $1/169$ for [independence](../../../../../independent-random-variables.md), forcing $17-16p=13$ and therefore

$$
\boxed{p=\frac14.}
$$

At this value the off-diagonal expression is also $1/169$, proving sufficiency for every ordered pair. This is an example of [match-biased reshuffling preserves uniform rank marginals](../../../../../match-biased-reshuffling-preserves-uniform-rank-marginals.md): state-dependent [rejection sampling](../../../../../rejection-sampling.md) changes dependence even though both individual rank distributions remain uniform.

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
