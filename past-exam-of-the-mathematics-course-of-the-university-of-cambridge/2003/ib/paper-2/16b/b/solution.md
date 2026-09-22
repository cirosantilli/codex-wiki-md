<h1 id="16b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $f=p(x)e^{-x^2/2}$. Differentiating gives

$$
f''-x^2f=[p''-2xp'-p]e^{-x^2/2}.
$$

Thus the [polynomial](../../../../../../polynomial-split.md) must satisfy $p''-2xp'-(\mu+1)p=0$. If it has degree $n$ and nonzero leading [coefficient](../../../../../../coefficient.md), comparison of highest powers gives $\mu=-(2n+1)$. For this value the equation becomes the [Hermite differential equation](../../../../../../hermite-differential-equation.md)

$$
p''-2xp'+2np=0.
$$

Write $p=\sum_{j=0}^na_jx^j$, with [coefficients](../../../../../../coefficient.md) beyond $n$ zero. Comparing powers yields

$$
(j+2)(j+1)a_{j+2}+2(n-j)a_j=0.
$$

The equation at $j=n-1$ forces $a_{n-1}=0$, and downward recurrence removes all terms of the opposite parity and determines all same-parity terms from $a_n$. Taking $a_n=1$ produces the explicit [polynomial](../../../../../../polynomial-split.md)

$$
p_n(x)=\sum_{r=0}^{\lfloor n/2\rfloor}
\frac{(-1)^r n!}{4^r r!(n-2r)!}x^{n-2r}.
$$

It satisfies every [coefficient](../../../../../../coefficient.md) equation, so existence as well as uniqueness up to a nonzero scalar is proved. Hence

$$
\boxed{\mu_n=-(2n+1),\qquad f_n=p_ne^{-x^2/2}.}
$$

The monic $p_n$ is $2^{-n}$ times the usual physicists' [Hermite polynomial](../../../../../../hermite-polynomial.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [16B](../../16b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
