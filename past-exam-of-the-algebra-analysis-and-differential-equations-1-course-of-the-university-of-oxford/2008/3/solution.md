<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Reduction modulo the prime $p$ preserves integer addition, multiplication, and one:

$$
\overline{a+b}=\bar a+\bar b,\qquad \overline{ab}=\bar a\bar b.
$$

Every congruence class has an integer representative, so the [ring homomorphism](../../../ring-homomorphism.md) is onto. Its kernel is exactly $p\mathbb Z=(p)$. The quotient is a field because every class not divisible by $p$ has a multiplicative inverse by [Bézout's identity](../../../bezout-s-identity.md).

For the coefficientwise extension to the [polynomial ring](../../../polynomial-ring.md), addition is preserved term by term. If $f=\sum_ia_ix^i$ and $g=\sum_jb_jx^j$, the coefficient of $x^k$ in their product is $\sum_{i+j=k}a_ib_j$. Reducing it modulo $p$ gives $\sum_{i+j=k}\bar a_i\bar b_j$, the coefficient in $\hat\phi(f)\hat\phi(g)$. Thus multiplication and one are preserved as well. Lift each coefficient of a polynomial over $\mathbb Z_p$ to an integer to prove surjectivity. The kernel is

$$
\boxed{\ker\hat\phi=p\mathbb Z[x]=(p).}
$$

Indeed, its elements are precisely the polynomials whose coefficients are all divisible by $p$.

In the [binomial theorem](../../../binomial-theorem.md) expansion of $(x-1)^p$, every intermediate coefficient $\binom pj$ is divisible by $p$: the numerator contains the prime factor $p$, while $j!(p-j)!$ does not for $1\leq j<p$. Hence

$$
(x-1)^p=x^p+(-1)^p=x^p-1\quad\text{in }\mathbb Z_p[x].
$$

For $p=2$, the last equality uses $1=-1$ in characteristic two. This is an instance of the [Frobenius endomorphism](../../../frobenius-endomorphism.md).

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2008](../../2008-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
