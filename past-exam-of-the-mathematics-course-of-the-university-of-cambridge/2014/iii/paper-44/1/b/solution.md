<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the normalized Gaussian integral with action $\operatorname{tr}(M^2)/2$. Its [Wick contraction](../../../../../../wick-contraction.md) is

$$
\langle M^i{}_j M^k{}_l\rangle_0=\delta^i{}_l\delta^k{}_j.
$$

There is no factor $1/N$ here: this part uses $V$, whereas the following part uses $NV$. Expanding the normalized [Hermitian matrix model](../../../../../../hermitian-matrix-model.md) integral to first order gives

$$
\langle M^i{}_j M^k{}_l\rangle
=\langle M^i{}_j M^k{}_l\rangle_0-\frac g4\left[
\langle M^i{}_j M^k{}_l\operatorname{tr}(M^4)\rangle_0
-\langle M^i{}_j M^k{}_l\rangle_0\langle\operatorname{tr}(M^4)\rangle_0\right]+O(g^2).
$$

The subtracted term removes [Vacuum Feynman diagrams](../../../../../../vacuum-feynman-diagram.md) disconnected from the external pair. Since the one-point function vanishes by $M\mapsto-M$, the resulting two-point function is a [connected correlation function](../../../../../../connected-correlation-function.md).

Write the vertex as $M^a{}_bM^b{}_cM^c{}_dM^d{}_a$. Each external field must contract with a different vertex field, leaving the other two to form a [tadpole diagram](../../../../../../tadpole-diagram.md). Eight of the twelve connected pairings attach the external fields at adjacent cyclic positions. The remaining index loop gives $N\delta^i{}_l\delta^k{}_j$ in each case. The other four attach them at opposite positions and give $\delta^i{}_j\delta^k{}_l$, with no free index loop. Therefore

$$
\boxed{\langle M^i{}_j M^k{}_l\rangle_c
=(1-2gN)\delta^i{}_l\delta^k{}_j-g\delta^i{}_j\delta^k{}_l+O(g^2).}
$$

**Both index structures are required at finite $N$**. For $N=1$ the answer is $1-3g+O(g^2)$, agreeing with the ordinary zero-dimensional quartic integral. This is a formal [perturbative quantum field theory](../../../../../../perturbative-quantum-field-theory-split.md) expansion; the real integral is convergent for $g\ge0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
