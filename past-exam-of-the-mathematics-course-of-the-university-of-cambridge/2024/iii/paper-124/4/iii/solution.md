<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

We give the [Agrawal–Biswas primality test](../../../../../../agrawal-biswas-primality-test.md), which has one-sided error. Small inputs and [perfect powers](../../../../../../perfect-power.md) can first be recognized deterministically. For every remaining integer $n$, put $d=\lceil4\log_2n\rceil$ and choose a uniformly random monic polynomial

$$
r(X)=X^d+a_{d-1}X^{d-1}+\cdots+a_0
\in(\mathbb Z/n\mathbb Z)[X].
$$

Using repeated squaring in the quotient ring $(\mathbb Z/n\mathbb Z)[X]/(r)$, test the [identity](../../../../../../polynomial-identity-testing.md)

$$
(X+1)^n\equiv X^n+1\pmod{n,r(X)}.
$$

This takes time polynomial in $\log n$ because every intermediate polynomial has degree below $d=O(\!\log n)$.

If $n$ is [prime](../../../../../../prime-number.md), the intermediate [binomial coefficients](../../../../../../binomial-coefficient.md) are divisible by $n$, so the identity always holds. Now suppose that $n$ is composite and is not a prime power. Choose a prime divisor $p$ and write $n=p^am$ with $p\nmid m$ and $m>1$. Over $\mathbb F_p$,

$$
(X+1)^n=(X^{p^a}+1)^m\ne X^n+1,
$$

because an intermediate coefficient equal to $m$ is nonzero modulo $p$. Hence

$$
F(X)=(X+1)^n-X^n-1
$$

is a nonzero polynomial of degree below $n$ over $\mathbb F_p$.

Reduction of random $r$ modulo $p$ is uniform among the $p^d$ monic degree-$d$ polynomials. The polynomial $F$ has at most $n/d$ distinct monic [irreducible](../../../../../../irreducible-polynomial.md) factors of degree $d$. On the other hand, the number $I_p(d)$ of monic irreducibles of degree $d$ obeys the standard lower bound

$$
I_p(d)\geq\frac{p^d}{d}-p^{d/2}.
$$

Whenever $r\bmod p$ is one of these irreducibles but does not divide $F$, the tested congruence fails. Thus one trial detects compositeness with probability at least

$$
\frac{I_p(d)-n/d}{p^d}
\geq\frac1d-p^{-d/2}-\frac{n}{dp^d}
\geq\frac1{2d}
$$

after the finitely many small $n$ are handled directly. Repeating $2d$ times makes the probability of missing a composite less than $(1-1/(2d))^{2d}<1/2$, while a prime is never rejected. Therefore compositeness is in [RP](../../../../../../rp-complexity.md), and primality testing is in

$$
\boxed{\mathbf{co\text{-}RP}.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
