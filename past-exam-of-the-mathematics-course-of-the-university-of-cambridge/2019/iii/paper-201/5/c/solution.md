<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because $f$ is a continuous probability density, there are a point $z$, a radius $r>0$, and $\epsilon>0$ such that

$$
f\geq\epsilon\quad\text{on }B(z,r).
$$

By the [recurrence of planar Brownian motion](../../../../../../recurrence-of-planar-brownian-motion.md), the smaller disc $B(z,r/2)$ is visited at arbitrarily large times. Starting anywhere in that smaller disc, Brownian continuity and compactness give a uniform probability $\delta>0$ of staying in $B(z,r)$ for a fixed time $u>0$.

Apply the [Strong Markov property](../../../../../../strong-markov-property.md) at successive visits separated by at least $u$. The conditional probability of each stay event is at least $\delta$, so the conditional [Borel-Cantelli lemma](../../../../../../borel-cantelli-lemmas.md) gives infinitely many successful stays almost surely. Every success adds at least $\epsilon u$ to $A_t$. Since $A_t$ is nondecreasing,

$$
\boxed{A_t\longrightarrow\infty\quad\text{almost surely}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
