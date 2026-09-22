<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [Fredholm operator](../../../../../../fredholm-operator.md) $T$, define $B$ to invert $T:(\ker T)^\perp\to\operatorname{ran}T$ and to vanish on the range complement. The [bounded inverse theorem](../../../../../../bounded-inverse-theorem.md) makes $B$ bounded, and

$$
BT=I-P_{\ker T},\qquad TB=I-P_{\ker T^*}.
$$

The errors are finite rank, so $T$ is invertible in the [Calkin algebra](../../../../../../calkin-algebra.md).

Conversely suppose $BT=I-K$ and $TB=I-L$ for bounded $B$ and compact $K,L$. On $\ker T$, $K$ is the identity. An infinite-dimensional closed kernel would contain an orthonormal sequence, whose images under $K$ have no convergent subsequence, contradicting compactness. Thus the kernel is finite-dimensional.

There is a positive lower bound for $T$ on $(\ker T)^\perp$. Otherwise choose unit vectors $x_j$ there with $Tx_j\to0$. Since $x_j=BTx_j+Kx_j$, compactness gives a norm-convergent subsequence with unit limit $x$. The limit lies in the kernel complement and has $Tx=0$, a contradiction. This lower bound proves closed range: if $Tx_j$ converges, remove each kernel component; the remaining $x_j$ form a [Cauchy sequence](../../../../../../cauchy-sequence.md) and converge to a preimage of the limit.

Finally adjointing $TB=I-L$ gives $B^*T^*=I-L^*$. The same kernel argument makes $\ker T^*$ finite-dimensional. Therefore $T$ is [Fredholm](../../../../../../fredholm-operator.md). **$\boxed{T\text{ is Fredholm}\iff[T]\text{ is invertible modulo compacts}}$**, the [Atkinson theorem](../../../../../../atkinson-theorem.md). The finite-dimensional case also satisfies the parametrix formulation directly, though its quotient algebra is the zero algebra.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
