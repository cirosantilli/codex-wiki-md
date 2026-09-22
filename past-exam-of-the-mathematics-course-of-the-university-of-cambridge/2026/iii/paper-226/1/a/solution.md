<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [simple random walk](../../../../../../simple-random-walk.md) on $\mathbb Z^d$, $d\geq3$, the [Green-function decay for simple random walk on the integer lattice](../../../../../../green-function-decay-for-simple-random-walk-on-the-integer-lattice.md) and the [Strong Markov property](../../../../../../strong-markov-property.md) give

$$
P_0(H_{\{x_k\}}<\infty)
=\frac{g(0,x_k)}{g(x_k,x_k)}
\leq C|x_k|^{2-d}
=C2^{-k(d-2)}.
$$

The series over $k$ converges, so the first of the [Borel-Cantelli lemmas](../../../../../../borel-cantelli-lemmas.md) says that almost surely only finitely many of the points $x_k$ are ever hit. Moreover, $\mathbb Z^d$ is a [transient graph](../../../../../../transient-graph.md) for $d\geq3$, so each of those finitely many points is visited only finitely often. Therefore the [simple random walk](../../../../../../simple-random-walk.md) visits $A$ only finitely often almost surely:

$$
\boxed{P_0(X_n\in A\text{ for infinitely many }n)=0.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 226](../../../paper-226-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
