<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a compact convex set $K\subset\mathbb R^n$, let

$$
H_K(\eta)=\sup_{x\in K}x\mathbin\cdot\eta.
$$

The [Paley–Wiener–Schwartz theorem](../../../../../../paley-wiener-schwartz-theorem.md) says that if $u$ is a [compactly supported distribution](../../../../../../compactly-supported-distribution.md) with support in $K$, its Fourier--Laplace transform

$$
\widehat u(z)=\langle u(x),e^{-ix\cdot z}\rangle
$$

is entire and, for some $C,N$,

$$
|\widehat u(z)|\leq C(1+|z|)^N
e^{H_K(\operatorname{Im}z)}.
$$

Conversely, every entire function satisfying such an estimate is the transform of a distribution supported in $K$.

For the forward direction, compact support lets $u$ act on the exponential after insertion of a cutoff equal to one near $K$. Differentiation in $z$ may be passed under the pairing, proving entire analyticity. The finite-order estimate for $u$ bounds derivatives of the exponential on $K$ by a polynomial in $|z|$ times $e^{H_K(\operatorname{Im}z)}$.

Conversely, restrict the entire function $F$ to $\mathbb R^n$. Its polynomial growth defines a [tempered distribution](../../../../../../tempered-distribution.md) $u$ by inverse [Fourier transform](../../../../../../fourier-transform.md). If a test function is supported outside $K$, separate its compact support from $K$ by a real vector $\eta$. Shifting the Fourier inversion contour from $\mathbb R^n$ to $\mathbb R^n+i t\eta$ is allowed by entire analyticity. The exponential gained from the test function beats the bound $e^{tH_K(\eta)}$ as $t\to\infty$, so the pairing vanishes. Hence $\operatorname{supp}u\subset K$, completing the converse.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 327](../../../paper-327-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
