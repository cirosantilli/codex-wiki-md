<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix a basis for the [transposition map](../../../../../../transpose.md) $T$. If $M\geq0$, write $M=BB^\dagger$. Then

$$
T(M)=M^T=\overline B B^T=\overline B(\overline B)^\dagger\geq0.
$$

Thus transposition is a [positive linear map](../../../../../../positive-linear-map.md) and also preserves the [trace](../../../../../../matrix-trace.md).

For dimension $D\geq2$, apply it to one subsystem of the [maximally entangled state](../../../../../../maximally-entangled-state.md) from part (a):

$$
(\operatorname{id}\otimes T)(|\Omega\rangle\langle\Omega|)
=\frac1D\sum_{i,j}|i\rangle\langle j|\otimes|j\rangle\langle i|
=\frac FD,
$$

where $F$ is the [swap operator](../../../../../../swap-operator.md), $F(|u\rangle\otimes|v\rangle)=|v\rangle\otimes|u\rangle$. It satisfies $F^\dagger=F$ and $F^2=I$, so its [eigenvalues](../../../../../../eigenvalue.md) are $+1$ on symmetric vectors and $-1$ on antisymmetric vectors. In particular,

$$
|\eta\rangle=\frac{|1\rangle|2\rangle-|2\rangle|1\rangle}{\sqrt2},
\qquad
\langle\eta|\frac FD|\eta\rangle=-\frac1D<0.
$$

A positive input has therefore acquired a negative expectation value after adjoining an identity channel. **Transposition is positive but not completely positive in dimension at least two.** The one-dimensional case is the identity map and is completely positive; the dimension qualification is necessary.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
