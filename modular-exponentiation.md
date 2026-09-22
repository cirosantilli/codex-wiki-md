# Modular exponentiation

↑ **Parent:** [Exponentiation by squaring](exponentiation-by-squaring.md)

Modular exponentiation computes the [remainder](remainder.md) $a^n\bmod m$ for an [integer](integer-split.md) base $a$, a [nonnegative integer](natural-number.md) exponent $n$, and, here, an [integer](integer-split.md) modulus $m\geq2$. It applies [exponentiation by squaring](exponentiation-by-squaring.md) while reducing after **each** [multiplication](multiplication.md), including each squaring. The result is the unique representative in $\{0,\ldots,m-1\}$. There is no requirement that the base be [coprime](coprime-integers.md) to the modulus when the exponent is nonnegative.[Section 3.4, pp. 64–66: canonical representatives, modular products, and nonnegative-exponent repeated squaring](a-computational-introduction-to-number-theory-and-algebra-by-victor-shoup.md)

Take $a=2$, $n=13=(1101)_2$, and $m=17$. Initialize $r=2$; the remaining digits give

$$
\begin{aligned}
11&:\quad 2^2\bmod17=4,\quad4\cdot2\bmod17=8,\\
110&:\quad 8^2\bmod17=64\bmod17=13,\\
1101&:\quad13^2\bmod17=169\bmod17=16,\quad16\cdot2\bmod17=15.
\end{aligned}
$$

Hence **$2^{13}\bmod17=15$**. The final operation multiplies $16$ by $2$, since the preceding square has already been reduced. The computation never needs to construct $2^{13}=8192$.

In general reduce the base first, $x=a\bmod m$. For $n>0$, initialize $r=x$ and process the remaining [binary digits](binary-digit.md) with $r\leftarrow r^2\bmod m$, followed, for a digit one, by $r\leftarrow rx\bmod m$. The [loop invariant](loop-invariant.md) is

$$
0\leq r<m,\qquad r\equiv a^p\pmod m,
$$

where $p$ is the processed prefix value. The congruence is preserved because [modular arithmetic](modular-arithmetic-split.md) respects [multiplication](multiplication.md): if $u\equiv v\pmod m$, then $u^2\equiv v^2$ and $ux\equiv va\pmod m$. Thus changing representatives never changes the final [congruence class](congruence-class.md).

Both factors in every product are less than $m$, so the unreduced product is less than $m^2$, and the stored result is again less than $m$. The same bounds hold for a gigantic exponent, such as $n=2^{1000}$: there are $1000$ squarings, each on bounded-size residues. For base two, the corresponding ordinary power would have $2^{1000}+1$ [binary digits](binary-digit.md). The benefit is avoiding the huge ordinary power altogether, rather than constructing it and taking one final [remainder](remainder.md). Initial reduction is essential when the supplied base is much larger than the modulus.

For $n=0$, return $1$ under the same empty-product convention as [exponentiation by squaring](exponentiation-by-squaring.md). For $n=-k<0$, require $\gcd(a,m)=1$, find the [modular multiplicative inverse](modular-multiplicative-inverse.md) $a^{-1}\bmod m$, and compute $(a^{-1})^k\bmod m$; the [extended Euclidean algorithm](extended-euclidean-algorithm.md) can find that inverse. Its cost is separate from the positive-exponent [binary powering multiplication count](binary-powering-multiplication-count.md). For example, $2^{-1}\equiv9\pmod{17}$, while $2^{-1}\bmod4$ is undefined because $2$ and $4$ are not [coprime](coprime-integers.md).

A [reversible computation](reversible-computation.md) gives the coherent [quantum modular exponentiation](quantum-modular-exponentiation.md) used in [quantum order finding](quantum-order-finding.md) and [discrete-logarithm Fourier sampling](discrete-logarithm-fourier-sampling.md).

**Table of contents**

- [Bit cost of modular exponentiation](bit-cost-of-modular-exponentiation.md)

## ↑ Ancestors (5)

1. [Exponentiation by squaring](exponentiation-by-squaring.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Bit cost of modular exponentiation](bit-cost-of-modular-exponentiation.md)
- [Carmichael function](carmichael-function.md)
- [Euler's criterion](euler-s-criterion.md)
- [Exponent reduction for units](exponent-reduction-for-units.md)
- [Exponentiation by squaring](exponentiation-by-squaring.md)
- [Fermat little theorem](fermat-little-theorem.md)
- [Fermat test example](fermat-test-example.md)
- [Modular arithmetic](modular-arithmetic-split.md)
- [Multiplicative order](multiplicative-order.md)
- [Order as the exact period of modular exponentiation](order-as-the-exact-period-of-modular-exponentiation.md)
- [Passing-base fraction for the Fermat test](passing-base-fraction-for-the-fermat-test.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/1/b/iii/solution.md)
- [Pépin's test](pepin-s-test.md)
- [Quadratic residue](quadratic-residue-split.md)
- [Residue class](residue-class.md)
