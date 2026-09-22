# Laplace transform of a Laguerre polynomial

↑ **Parent:** [Laguerre polynomial](laguerre-polynomial.md)

For the ordinary [Laguerre polynomial](laguerre-polynomial.md) $L_n(t)=\sum_{j=0}^n\binom nj(-t)^j/j!$, apply the [Laplace transform](laplace-transform.md) to each term, using $\mathcal L[t^j](p)=j!/p^{j+1}$ for $\operatorname{Re}p>0$. The [binomial theorem](binomial-theorem.md) gives

$$
\mathcal L[L_n](p)=\frac1p\sum_{j=0}^n\binom nj(-p^{-1})^j=\frac1p(1-p^{-1})^n.
$$

This proves the formula for every nonnegative [integer](integer-split.md) $n$. In particular $L_2(t)=1-2t+t^2/2$ has transform $(p-1)^2/p^3$.

## ↑ Ancestors (9)

1. [Laguerre polynomial](laguerre-polynomial.md)
2. [Laguerre differential operator on polynomials](laguerre-differential-operator-on-polynomials.md)
3. [Self-adjoint operator](self-adjoint-operator.md)
4. [Operator theory](linear-operator-theory-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2/5/solution.md)
