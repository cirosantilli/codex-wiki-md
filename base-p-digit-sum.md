# Base-p digit sum

↑ **Parent:** [P-adic valuation](p-adic-valuation.md)

For a [nonnegative integer](natural-number.md) $n$ and [integer](integer-split.md) base $p\geq2$, write its [base-p expansion](base-p-expansion.md) as

$$
n=\sum_{r\geq0}\alpha_rp^r,
\qquad 0\leq\alpha_r<p,
$$

The base-$p$ digit sum is $d_p(n)=\sum_r\alpha_r$, with $d_p(0)=0$. When $p$ is a [prime number](prime-number-split.md), the [Legendre formula](legendre-s-formula.md) becomes

$$
v_p(n!)=\frac{n-d_p(n)}{p-1}.
$$

To see the connection, divide the [base-p expansion](base-p-expansion.md) by $p^j$ and discard the fractional part. Swapping the resulting finite sums and using a [finite geometric series](finite-geometric-series.md) gives

$$
\sum_{j\geq1}\left\lfloor\frac n{p^j}\right\rfloor
=\sum_{r\geq1}\alpha_r\sum_{j=1}^r p^{r-j}
=\sum_{r\geq0}\alpha_r\frac{p^r-1}{p-1}
=\frac{n-d_p(n)}{p-1}.
$$

In particular, $50=1\cdot27+2\cdot9+1\cdot3+2=(1212)_3$, so $d_3(50)=6$ and $v_3(50!)=(50-6)/2=22$. The leading [numeral digit](numerical-digit.md) contributes thirteen, the next contributes eight, the next one, and the units contribute zero. Thus the [base-p digit sum](base-p-digit-sum.md) compresses the same contribution ledger into information already present in [positional notation](positional-notation.md).

**Table of contents**

- [Subadditivity of the base-p digit sum](subadditivity-of-the-base-p-digit-sum.md)

## ↑ Ancestors (5)

1. [P-adic valuation](p-adic-valuation.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Balanced number](balanced-number.md)
- [Base-p digit sum](base-p-digit-sum.md)
- [Harshad number](harshad-number.md)
- [Kummer's theorem](kummer-s-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-103/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-103/4/ii/solution.md)
- [Subadditivity of the base-p digit sum](subadditivity-of-the-base-p-digit-sum.md)
