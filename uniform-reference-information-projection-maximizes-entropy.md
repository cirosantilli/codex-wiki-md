# Uniform-reference information projection maximizes entropy

↑ **Parent:** [Information projection](information-projection.md)

For a [uniform distribution on a finite set](discrete-uniform-distribution.md) of $m$ outcomes, direct expansion of [relative entropy](kullback-leibler-divergence.md) gives

$$
D(q\Vert u)=\sum_i q_i\ln(mq_i)=\ln m-H_e(q),
$$

where $H_e$ is [information entropy](information-entropy.md) in [nats](nat-unit.md). Therefore minimizing [relative entropy](kullback-leibler-divergence.md) from this particular reference is equivalent to maximizing [information entropy](information-entropy.md) subject to the same constraint. This statement depends on the uniform reference; an arbitrary reference contributes its own weights.

In the three-outcome example, $H_e(q^*)=\ln3-D(q^*\Vert p)\approx0.901235$ [nats](nat-unit.md). The [mean](expected-value.md) fixes one aggregate quantity, and [information projection](information-projection.md) chooses how to distribute the remaining uncertainty. This extends [maximum entropy on a finite alphabet](maximum-entropy-on-a-finite-alphabet.md), whose unconstrained maximizer is the uniform law itself.

## ↑ Ancestors (8)

1. [Information projection](information-projection.md)
2. [Method of types](method-of-types.md)
3. [Type (information theory)](type-information-theory.md)
4. [Information theory](information-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
