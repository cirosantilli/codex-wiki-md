# Kravchuk polynomials

↑ **Parent:** [Orthogonal polynomial](orthogonal-polynomial.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kravchuk_polynomials)

These [polynomials](polynomial-split.md) are orthogonal for a [binomial distribution](binomial-distribution.md) weight and encode the coefficient transformation in the [MacWilliams identity](macwilliams-identity.md). Their [generating function](generating-function.md) follows by expanding the two factors:

$$
\sum_{s=0}^nK_s(t;n,q)z^s=(1-z)^t(1+(q-1)z)^{n-t}.
$$

For binary [linear codes](linear-code.md), $q=2$. Expanding the factors gives $K_s(t;n,2)=\sum_j(-1)^j\binom tj\binom{n-t}{s-j}$, where [binomial coefficients](binomial-coefficient.md) outside their usual integer range are zero. Orthogonality follows by multiplying [generating functions](generating-function.md) and summing over $t$ with weight $\binom nt(q-1)^t$: the result is $q^n(1+(q-1)zw)^n$, whose coefficient of $z^rw^s$ is zero for $r\ne s$ and $q^n(q-1)^r\binom nr$ for $r=s$.

## ↑ Ancestors (6)

1. [Orthogonal polynomial](orthogonal-polynomial.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-30/2/solution.md)
