<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

Work with well-ordered cardinals, as usual with the [axiom of choice](../../../../../axiom-of-choice.md). We first prove the infinite [cardinal arithmetic](../../../../../cardinal-arithmetic.md) identity $\kappa^2=\kappa$. If a least infinite counterexample $\kappa$ existed, order pairs of ordinals below $\kappa$ first by their maximum coordinate, then lexicographically within each level. Every initial segment ending at $(\xi,\eta)$ lies inside $(\max(\xi,\eta)+1)^2$. Its cardinal is less than $\kappa$, by the smaller-cardinal identity or finite counting. This well-order cannot have an element with $\kappa$ predecessors, so its order type is at most the initial ordinal $\kappa$. Thus $|\kappa\times\kappa|\leq\kappa$, contrary to its being a counterexample; the reverse injection is $\xi\mapsto(\xi,0)$. Hence

$$
\boxed{\aleph_\alpha^2=\aleph_\alpha\quad\text{for every }\alpha.}
$$

A sum of finitely many finite cardinals is finite, so **$\aleph_0$ is regular**. A sum of fewer than $\aleph_1$ smaller cardinals is a countable union of countable sets and has size at most $\aleph_0^2=\aleph_0$, so **$\aleph_1$ is regular**.

Likewise fewer than $\aleph_2$ summands means at most $\aleph_1$ summands, each of size at most $\aleph_1$. Their sum is at most $\aleph_1^2=\aleph_1<\aleph_2$. Thus **$\aleph_2$ is regular**. In contrast,

$$
\aleph_\omega=\sum_{n<\omega}\aleph_n
$$

is a countable sum of smaller cardinals, with $\aleph_0<\aleph_\omega$. Therefore **$\aleph_\omega$ is singular**, of [cofinality](../../../../../cofinality.md) $\omega$.

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
