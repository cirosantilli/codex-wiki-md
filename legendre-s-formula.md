<h1 id="legendre-s-formula">Legendre's formula</h1>

↑ **Parent:** [P-adic valuation](p-adic-valuation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Legendre's_formula)

For a [nonnegative integer](natural-number.md) $n$ and a [prime number](prime-number-split.md) $p$, the [Legendre formula](legendre-s-formula.md) computes the [prime exponent](p-adic-valuation.md) in a [factorial](factorial.md) without forming that huge product:

$$
v_p(n!)=\sum_{j\geq1}\left\lfloor\frac{n}{p^j}\right\rfloor.
$$

Here $\lfloor x\rfloor$ is the [floor function](floor-function.md). The sum is finite: every term with $p^j>n$ is zero. When $n=0$, all terms vanish, agreeing with $0!=1$ and $v_p(1)=0$. The [prime number](prime-number-split.md) hypothesis matters: a [composite number](composite-number.md) does not give the same [P-adic valuation](p-adic-valuation.md) or additive [prime exponent](p-adic-valuation.md). For example, the floor sum with $n=6,p=4$ is one, whereas $4^2$ divides $6!=720$.

Why count multiples repeatedly? Each multiple of $p$ in $1,\ldots,n$ contributes one factor of $p$; each multiple of $p^2$ contributes another; and so on. A factor $m$ with [P-adic valuation](p-adic-valuation.md) $a$ occurs in exactly the first $a$ counts. Adding those contributions proves the formula.[David A. Santos, Number Theory for Mathematical Contests, revision 31 October 2007, §8.3, Theorem 245, printed pp. 89–90: factorial valuation and digit form](number-theory-for-mathematical-contests-by-david-anthony-santos.md)

For the original example $n=50,p=3$,

$$
v_3(50!)=\left\lfloor\frac{50}{3}\right\rfloor+
\left\lfloor\frac{50}{9}\right\rfloor+
\left\lfloor\frac{50}{27}\right\rfloor
=16+5+1=22.
$$

The five multiples $9,18,27,36,45$ each contribute a second factor of three. The factor $27$ contributes a third, so it appears in all three rows. Equivalently, among $1,\ldots,50$ there are eleven factors of [P-adic valuation](p-adic-valuation.md) one, four of valuation two, and one of valuation three: $11+2\cdot4+3\cdot1=22$. Thus $3^{22}$ divides $50!$, while $3^{23}$ does not.

<a id="image-nested-multiples-count-the-factors-of-three-in-50"></a>
![](legendre-factorial-nested-multiples-ledger.png)

**[Figure 15](#image-nested-multiples-count-the-factors-of-three-in-50). Nested multiples count the factors of three in $50!$**. Each colored cell contributes one to the [P-adic valuation](p-adic-valuation.md). Multiples of nine occur in two rows, and $27$ occurs in three. Summing by rows gives $16+5+1$; summing by columns gives $11\cdot1+4\cdot2+1\cdot3$. Factors not divisible by three contribute zero and are omitted.

Repeated [Euclidean division](euclidean-division.md) provides a practical evaluation: replace $q$ by $\lfloor q/p\rfloor$, starting from $q=n$, and add each new quotient until it is zero. This uses only the successive quotients $16,5,1,0$ for the example. The same calculation handles [divisibility](divisibility-split.md) of [binomial coefficients](binomial-coefficient-split.md), where the [P-adic valuations](p-adic-valuation.md) of the denominator [factorials](factorial.md) are subtracted.

## ↑ Ancestors (5)

1. [P-adic valuation](p-adic-valuation.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
