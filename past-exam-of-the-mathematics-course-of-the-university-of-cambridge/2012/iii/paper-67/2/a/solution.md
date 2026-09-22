<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the bit-query [Boolean quantum oracle](../../../../../../boolean-quantum-oracle.md) $O_x|i,b,z\rangle=|i,b\mathbin\oplus x_i,z\rangle$, where $z$ denotes workspace. Initially every [probability amplitude](../../../../../../probability-amplitude.md) is independent of $x$, hence is a constant [polynomial](../../../../../../polynomial-split.md). An input-independent [unitary gate](../../../../../../quantum-logic-gate.md) only forms linear combinations of [probability amplitudes](../../../../../../probability-amplitude.md), so it does not increase their [polynomial degree](../../../../../../degree-of-a-polynomial.md).

If $a_{i,b,z}(x)$ is an amplitude before a query, its new value is

$$
a'_{i,b,z}(x)=(1-x_i)a_{i,b,z}(x)+x_i a_{i,b\oplus1,z}(x).
$$

One query increases [polynomial degree](../../../../../../degree-of-a-polynomial.md) by at most one. Inductively, after $T$ queries each amplitude has [polynomial degree](../../../../../../degree-of-a-polynomial.md) at most $T$. The acceptance [probability](../../../../../../probability.md) is a sum of squared absolute values of the accepting amplitudes, so it is a real [polynomial](../../../../../../polynomial-split.md) of degree at most $2T$. Intermediate [measurement in quantum measurements](../../../../../../quantum-measurement-split.md) and classical adaptation can be retained coherently, or handled by summing unnormalized branch probabilities; either approach yields the same degree bound.

An exact algorithm has acceptance [probability](../../../../../../probability.md) precisely $f(x)$ at every Boolean input. The [multilinear reduction on the Boolean cube](../../../../../../multilinear-reduction-on-the-boolean-cube.md) replaces positive powers of each $x_i$ by $x_i$, preserving these values without increasing [polynomial degree](../../../../../../degree-of-a-polynomial.md). Therefore the [polynomial method for quantum query lower bounds](../../../../../../polynomial-method-for-quantum-query-lower-bounds.md) gives

$$
\boxed{\deg(f)\le2T,\qquad Q_E(f)\ge\left\lceil\frac{\deg(f)}2\right\rceil.}
$$

Here $\deg(f)$ is the degree of the unique [multilinear polynomial](../../../../../../multilinear-polynomial.md) representing the [Boolean function](../../../../../../boolean-function.md), and $Q_E$ is its [exact quantum query complexity](../../../../../../exact-quantum-query-complexity.md). Uniqueness follows, for example, by evaluating successively on the indicator vectors of subsets: the value on a subset determines its coefficient once all smaller-subset coefficients are known.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
