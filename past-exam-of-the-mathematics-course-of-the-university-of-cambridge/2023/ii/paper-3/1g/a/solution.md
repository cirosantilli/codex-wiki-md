<h1 id="1g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [binomial theorem](../../../../../../binomial-theorem.md) gives

$$
4^n=(1+1)^{2n}=\sum_{k=0}^{2n}\binom{2n}{k}.
$$

The [central binomial coefficient](../../../../../../central-binomial-coefficient.md) is the largest of these $2n+1$ nonnegative [binomial coefficients](../../../../../../binomial-coefficient.md), so

$$
\binom{2n}{n}\geq\frac{4^n}{2n+1}=
\frac{2^{2n}}{2n+1}.
$$

For the upper bound, fix a [prime number](../../../../../../prime-number.md) $p\leq2n$. By [Legendre formula](../../../../../../legendre-s-formula.md),

$$
v_p\!\left(\binom{2n}{n}\right)
=\sum_{j\geq1}
\left(
\left\lfloor\frac{2n}{p^j}\right\rfloor
-2\left\lfloor\frac{n}{p^j}\right\rfloor
\right).
$$

Each summand is either zero or one. Hence the [P-adic valuation](../../../../../../p-adic-valuation.md) satisfies

$$
v_p\!\left(\binom{2n}{n}\right)
\leq\left\lfloor\frac{\log(2n)}{\log p}\right\rfloor.
$$

If $p\leq\sqrt{2n}$, this implies

$$
p^{v_p(\binom{2n}{n})}\leq2n.
$$

There are at most $\sqrt{2n}$ such [prime numbers](../../../../../../prime-number.md). If instead $p>\sqrt{2n}$, then $p^2>2n$, so the [P-adic valuation](../../../../../../p-adic-valuation.md) is at most one. Multiplying the prime-power contributions therefore yields

$$
\binom{2n}{n}
\leq(2n)^{\sqrt{2n}}
\prod_{\substack{p\leq2n\\p\text{ prime}}}p.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1G](../../1g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
