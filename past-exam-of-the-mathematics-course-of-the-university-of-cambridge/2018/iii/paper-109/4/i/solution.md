<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $D_n(a)$ denote the [constant term](../../../../../../constant-term.md), retaining the dimension as a subscript when it changes. We use the [Good recurrence for the Dyson constant term](../../../../../../good-recurrence-for-the-dyson-constant-term.md). For algebraically independent variables, [Lagrange interpolation polynomial](../../../../../../lagrange-polynomial.md) applied to the constant polynomial one gives

$$
1=\sum_{i=1}^n\prod_{j\ne i}\frac{t-X_j}{X_i-X_j}.
$$

At $t=0$, this becomes the rational identity

$$
1=\sum_{i=1}^n\prod_{j\ne i}\left(1-\frac{X_i}{X_j}\right)^{-1}.
$$

When every $a_i>0$, multiplying by the given [Laurent polynomial](../../../../../../laurent-polynomial.md) cancels one factor in row $i$ of the product and gives

$$
F(X;a)=\sum_{i=1}^n F(X;a-e_i),\qquad D_n(a)=\sum_{i=1}^n D_n(a-e_i).
$$

This is a polynomial identity after cancellation; no choice of an expansion of a rational function is involved.

The boundary case is essential. If $a_i=0$, the factors in row $i$ are absent. The only factors involving $X_i$ are then $(1-X_j/X_i)^{a_j}$ for $j\ne i$, and all their powers of $X_i$ are nonpositive. To obtain power zero in $X_i$, one must select the [constant term](../../../../../../constant-term.md) one from each of them. Taking the [constant term](../../../../../../constant-term.md) in $X_i$ therefore deletes that variable and exponent:

$$
D_n(a)=D_{n-1}(a_1,\ldots,\widehat{a_i},\ldots,a_n)\qquad(a_i=0).
$$

For $n=1$, the empty product is one, so $D_1(a_1)=1$. The all-zero exponent vector also gives one.

Now put $M_n(a)=m!/\prod_i a_i!$, where $m=\sum_i a_i$. This [multinomial coefficient](../../../../../../multinomial-coefficient.md) obeys the same deletion rule for a zero exponent. For positive exponents,

$$
\sum_i M_n(a-e_i)=\sum_i\frac{a_i}{m}M_n(a)=M_n(a).
$$

Induction on $n$, and within each dimension on $m$, consequently determines $D_n$ uniquely and identifies it with $M_n$. This proves the [Dyson constant-term identity](../../../../../../dyson-constant-term-identity.md):

$$
\boxed{D(a)=\frac{m!}{a_1!\cdots a_n!}=\binom{m}{a_1,\ldots,a_n}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
