<h1 id="9f/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $S=X+Y$ and $D=X-Y$. Since they are independent, applying the product rule for [moment-generating functions](../../../../../../moment-generating-function.md) to $S+D=2X$ gives

$$
M(2t)=M_S(t)M_D(t)=M(t)^2M(t)M(-t)=\boxed{M(t)^3M(-t)}.
$$

All factors are finite and strictly positive for every real $t$ by the stated hypothesis. Applying the same identity to $-t$ and dividing yields $\psi(2t)=\psi(t)^2$, or

$$
\boxed{\psi(t)=\psi(t/2)^2},\qquad \psi(t)=\frac{M(t)}{M(-t)}.
$$

The centered unit-variance [Taylor expansion](../../../../../../taylor-expansion.md) from part (ii) gives $M(h)=1+h^2/2+o(h^2)$ and the same expansion for $M(-h)$. Consequently $\psi(h)=1+o(h^2)$.

For the first step of [dyadic rigidity of a moment-generating function](../../../../../../dyadic-rigidity-of-a-moment-generating-function.md), take logarithms, which are allowed because $\psi>0$. For each fixed $t$ and every integer $m$,

$$
\log\psi(t)=2^m\log\psi(t/2^m).
$$

Since $\log\psi(h)=o(h^2)$, the right side tends to zero: it is $2^m o(t^2/4^m)$. Thus $\psi(t)=1$ for every $t$, and the [moment-generating function](../../../../../../moment-generating-function.md) is even.

The original identity now becomes $M(2t)=M(t)^4$. Iterating this time with the correct fourth-power scaling gives

$$
\log M(t)=4^m\log M(t/2^m).
$$

Near zero, $\log M(h)=h^2/2+o(h^2)$, so the right side tends to $t^2/2$. Therefore

$$
\boxed{M(t)=e^{t^2/2}\quad\text{for all real }t}.
$$

This is the [moment-generating function of a standard normal variable](../../../../../../moment-generating-function-of-a-standard-normal-variable.md). By the [uniqueness theorem for moment-generating functions](../../../../../../uniqueness-theorem-for-moment-generating-functions.md), each of $X$ and $Y$ has the [standard normal distribution](../../../../../../standard-normal-distribution.md). The proof establishes the [Gaussian characterization by independent sum and difference](../../../../../../gaussian-characterization-by-independent-sum-and-difference.md) directly from the two functional identities and the first two moments.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
