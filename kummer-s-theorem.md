<h1 id="kummer-s-theorem">Kummer's theorem</h1>

↑ **Parent:** [P-adic valuation](p-adic-valuation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kummer's_theorem)

For a [prime number](prime-number-split.md) $p$ and [integers](integer-split.md) $0\leq k\leq n$, the [P-adic valuation](p-adic-valuation.md) of the [binomial coefficient](binomial-coefficient-split.md) $\binom nk$ equals the number of [arithmetic carries](carry-arithmetic.md) in the base-$p$ [addition](addition.md) of $k$ and $n-k$.[David A. Santos, Number Theory for Mathematical Contests, revision 31 October 2007, §8.3, Theorem 246, printed p. 90: carry count for a binomial coefficient](number-theory-for-mathematical-contests-by-david-anthony-santos.md) Indeed, subtract the two denominator [factorial](factorial.md) valuations in the [Legendre formula](legendre-s-formula.md):

$$
v_p\binom nk=v_p(n!)-v_p(k!)-v_p((n-k)!)
=\frac{d_p(k)+d_p(n-k)-d_p(n)}{p-1}.
$$

Each [arithmetic carry](carry-arithmetic.md) accounts for one unit of this quotient by [subadditivity of the base-p digit sum](subadditivity-of-the-base-p-digit-sum.md). In particular, the [binomial coefficient](binomial-coefficient-split.md) is divisible by $p$ exactly when at least one carry occurs.

For $n=50,k=17,p=3$, the [factorial](factorial.md) counts give

$$
v_3\binom{50}{17}=22-(5+1)-(11+3+1)=1.
$$

The matching [base-p expansions](base-p-expansion.md) are $17=(0122)_3$ and $33=(1020)_3$. Their units add to two; the next column gives $2+2=4=1+3$, sending one carry into the nines column. That column then gives $1+0+1=2$, and no further carry occurs. The result is $(1212)_3=50$. The [base-p digit sums](base-p-digit-sum.md) check the same result: $(5+3-6)/(3-1)=1$. Consequently $\binom{50}{17}$ is divisible by three but not by nine.

<a id="image-the-base-p-digit-sum-and-one-arithmetic-carry-recover-the-same-prime-exponents"></a>
![](legendre-base-three-digits-and-carry.png)

**[Figure 16](#image-the-base-p-digit-sum-and-one-arithmetic-carry-recover-the-same-prime-exponents). The base-p digit sum and one arithmetic carry recover the same prime exponents**. On the left, the [base-p expansion](base-p-expansion.md) $50=(1212)_3$ gives $v_3(50!)=(50-6)/2=22$. On the right, $(0122)_3+(1020)_3=(1212)_3$ has exactly one carry, from the threes column into the nines column. [Kummer's theorem](kummer-s-theorem.md) therefore gives $v_3\binom{50}{17}=1$.

## ↑ Ancestors (5)

1. [P-adic valuation](p-adic-valuation.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Kummer's theorem](kummer-s-theorem.md)
- [Subadditivity of the base-p digit sum](subadditivity-of-the-base-p-digit-sum.md)
