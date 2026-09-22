<h1 id="26j/solution">Solution</h1>

↑ **Parent:** [26J](../26j.md)

[Kolmogorov zero-one law](../../../../../kolmogorov-s-zero-one-law.md) says that the tail sigma-algebra of [independent random variables](../../../../../independent-random-variables.md) is trivial: every tail event has probability zero or one. The [Birkhoff ergodic theorem](../../../../../birkhoff-ergodic-theorem.md) says that for a probability-preserving transformation $T$ and integrable $f$, the averages $A_nf=n^{-1}\sum_{j=0}^{n-1}f\circ T^j$ converge almost surely to $\mathbb E(f\mid\mathcal I)$, where $\mathcal I$ is the invariant sigma-algebra. The [mean ergodic theorem](../../../../../von-neumann-mean-ergodic-theorem.md) in $L^p$, $1\leq p<\infty$, gives the same convergence in $L^p$ for $f\in L^p$; $p=2$ is the classical von Neumann theorem, and on a probability space the $L^1$ version applies to the integrable case needed here. There is no general supremum-norm convergence assertion for $p=\infty$.

The [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) for iid integrable variables is $n^{-1}\sum_{j=1}^nX_j\to\mathbb EX_1$ almost surely. To prove it, realize the sequence on its product probability space and take the left shift $T$. The shift preserves the iid product law. Birkhoff applied to $f=X_1$ gives an almost-sure invariant limit $Z$. An invariant event is, modulo null sets, measurable with respect to coordinates after every finite index, hence is a tail event. Kolmogorov's law makes the invariant sigma-algebra trivial, so $Z$ is constant almost surely. Finally the $L^1$ mean ergodic theorem permits passing [expectations](../../../../../expected-value.md) through the limit; all averages have [expectation](../../../../../expected-value.md) $\mathbb EX_1$. This identifies that constant and proves the strong law.

## ↑ Ancestors (10)

1. [26J](../26j.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
