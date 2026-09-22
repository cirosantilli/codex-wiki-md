# Computing Legendre symbols by quadratic reciprocity

↑ **Parent:** [Quadratic reciprocity](quadratic-reciprocity.md)

The practical reward of [quadratic reciprocity](quadratic-reciprocity.md) is a smaller modulus: swap a pair of distinct [odd primes](odd-prime.md), record the required sign, then reduce the numerator by [modular arithmetic](modular-arithmetic.md). Use [multiplicativity of the Legendre symbol](multiplicativity-of-the-legendre-symbol.md) and the [second supplementary law for quadratic reciprocity](second-supplementary-law-for-quadratic-reciprocity.md) to handle a factor of two. For example,

$$
\begin{aligned}
\left(\frac{11}{43}\right)
&=-\left(\frac{43}{11}\right)
=-\left(\frac{10}{11}\right)
=-\left(\frac2{11}\right)\left(\frac5{11}\right)\\
&=\left(\frac5{11}\right)
=\left(\frac{11}{5}\right)
=\left(\frac15\right)=1.
\end{aligned}
$$

Here $11,43$ are both $3$ modulo $4$, so the first swap changes sign; $11\equiv3\pmod8$ gives $(2/11)=-1$; the swap involving five has no sign change. An independent square check is $21^2=441\equiv11\pmod{43}$. The method determines existence of a [square root](square-root.md) without itself finding that root.

A composite numerator is allowed in a [Legendre symbol](legendre-symbol.md); a composite denominator instead calls for a [Jacobi symbol](jacobi-symbol.md). Its [Jacobi reciprocity law](jacobi-reciprocity-law.md) supports repeated swaps and remainder reductions, in the spirit of the [Euclidean algorithm](euclidean-algorithm.md).[Ben Lynn, Quadratic Reciprocity, “The Jacobi Symbol”: product definition and reciprocity for computing symbols without factoring](quadratic-reciprocity-by-ben-lynn.md)

A final [Jacobi symbol](jacobi-symbol.md) of one is not a square-existence certificate for a [composite number](composite-number.md) modulus. For example,

$$
\left(\frac2{15}\right)=\left(\frac23\right)\left(\frac25\right)=(-1)(-1)=1,
$$

yet $x^2\equiv2\pmod{15}$ is impossible: reducing it modulo three would require a square congruent to two, and squares modulo three are only zero or one. The product has hidden two local failures. By contrast, for a [prime](prime-number.md) denominator, a [Legendre symbol](legendre-symbol.md) of one does certify a [quadratic residue](quadratic-residue.md).

## ↑ Ancestors (5)

1. [Quadratic reciprocity](quadratic-reciprocity.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
