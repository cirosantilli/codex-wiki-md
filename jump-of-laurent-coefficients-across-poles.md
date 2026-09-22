# Jump of Laurent coefficients across poles

↑ **Parent:** [Laurent coefficient](laurent-coefficient.md)

Suppose a [meromorphic function](meromorphic-function.md) is [holomorphic](holomorphic-function-split.md) on two concentric [annuli](annulus-mathematics.md) about $a$, with only finitely many [poles](pole.md) between chosen inner and outer coefficient circles. Let $a_n,b_n$ denote the corresponding [Laurent coefficients](laurent-coefficient.md). Subtract their [contour integral](contour-integral.md) formulas and apply the [residue theorem](residue-theorem.md) to the intervening annular region. It gives

$$
b_n-a_n=\sum_\zeta\operatorname{Res}_{z=\zeta}\frac{f(z)}{(z-a)^{n+1}}.
$$

The sum is over the [poles](pole.md) crossed, including their multiplicities through the [residue](residue.md). This identity applies to every integer index. Thus changing the [annulus](annulus-mathematics.md) can change even the coefficients of nonnegative powers; it is not merely a change in the [principal part](principal-part-of-a-meromorphic-function.md).

For example, $f(z)=1/\sin z$ has [simple poles](simple-pole.md) at $\pm\pi$, each with [residue](residue.md) $-1$. Moving a coefficient circle centered at zero from radius below $\pi$ to radius between $\pi$ and $2\pi$ changes its $n$th coefficient by $-\pi^{-n-1}-(-\pi)^{-n-1}$. Even indices remain unchanged, while odd indices acquire a nonzero correction.

## ↑ Ancestors (6)

1. [Laurent coefficient](laurent-coefficient.md)
2. [Laurent series](laurent-series.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
