<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $(\mathcal F_n)$ be the [natural filtration](../../../../../../natural-filtration.md) of the [random walk on a graph](../../../../../../random-walk-on-a-graph.md). For a bounded [harmonic function on a graph](../../../../../../discrete-harmonic-function.md), the transition rule and the [Markov property](../../../../../../markov-property.md) give

$$
\mathbb E[h(X_{n+1})\mid\mathcal F_n]
=\frac1{\deg(X_n)}\sum_{u\sim X_n}h(u)=h(X_n).
$$

Thus $h(X_n)$ is a bounded [martingale](../../../../../../martingale-split.md). The [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md) gives a finite almost sure limit $L$.

On the probability-one recurrence event, every vertex $v$ is visited along a sequence $n_k\to\infty$. Along that sequence $h(X_{n_k})=h(v)$, while convergence of the whole sequence forces $h(v)=L$. Therefore every pair of vertices has the same value. This is the [bounded harmonic function theorem on a recurrent graph](../../../../../../bounded-harmonic-function-theorem-on-a-recurrent-graph.md):

$$
\boxed{h(v)=h(w)\quad\text{for all vertices }v,w.}
$$

**Recurrence makes each vertex value a subsequential limit of the same convergent martingale.** A connected [locally finite graph](../../../../../../locally-finite-graph.md) is countable, since it is the union of its finite distance balls, so these almost sure assertions can also be combined by a countable intersection. The one-vertex case is immediate.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
