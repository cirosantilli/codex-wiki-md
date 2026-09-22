# Identity for Dirichlet convolution

↑ **Parent:** [Dirichlet convolution](dirichlet-convolution.md)

The [Identity for Dirichlet convolution](identity-for-dirichlet-convolution.md) is the [arithmetic function](arithmetic-function-split.md)

$$
\varepsilon(n)=\begin{cases}1&n=1,\\0&n>1.\end{cases}
$$

For every [arithmetic function](arithmetic-function-split.md) $f$, it satisfies $f*\varepsilon=\varepsilon*f=f$. Indeed, in $(f*\varepsilon)(n)=\sum_{d\mid n}f(d)\varepsilon(n/d)$, only $d=n$ survives. For example,

$$
(f*\varepsilon)(12)=f(1)0+f(2)0+f(3)0+f(4)0+f(6)0+f(12)1=f(12).
$$

At $n=1$ the sole term is $f(1)\varepsilon(1)=f(1)$. This gives a useful way to check [Dirichlet convolution](dirichlet-convolution.md) calculations: inserting $\varepsilon$ leaves every value unchanged. The three [arithmetic functions](arithmetic-function-split.md) $\mathbf1$, $\operatorname{id}$, and $\varepsilon$ all take value $1$ at $1$, but at $12$ the [constant-one arithmetic function](constant-one-arithmetic-function.md), the [identity arithmetic function](identity-arithmetic-function.md), and the [Identity for Dirichlet convolution](identity-for-dirichlet-convolution.md) take values $1$, $12$, and $0$, respectively. [Darij Grinberg, MIT 18.781 lecture notes, Theorem 2.3.4](https://darijgrinberg.gitlab.io/floor.pdf)

The [Möbius function](mobius-function.md) is the inverse of the [constant-one arithmetic function](constant-one-arithmetic-function.md) under [Dirichlet convolution](dirichlet-convolution.md), meaning $\mu*\mathbf1=\mathbf1*\mu=\varepsilon$. The [Möbius divisor-sum identity](mobius-divisor-sum-identity.md) gives a short proof: for $n>1$ the nonzero terms expand $\prod_{p\mid n}(1-1)=0$, while at $1$ the sum is $\mu(1)=1$. At $12$, the computation is

$$
(\mu*\mathbf1)(12)=\mu(1)+\mu(2)+\mu(3)+\mu(4)+\mu(6)+\mu(12)=1-1-1+0+1+0=0=\varepsilon(12).
$$

The zeros occur because $4$ and $12$ are divisible by the square of the [prime number](prime-number-split.md) $2$. Consequently, if $F=f*\mathbf1$ is a [divisor sum](divisor-sum.md), then [associativity](associative-property.md) gives $F*\mu=f*(\mathbf1*\mu)=f*\varepsilon=f$: this is [Möbius inversion](mobius-inversion-formula.md).

## ↑ Ancestors (6)

1. [Dirichlet convolution](dirichlet-convolution.md)
2. [Arithmetic function](arithmetic-function-split.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Constant-one arithmetic function](constant-one-arithmetic-function.md)
- [Dirichlet convolution](dirichlet-convolution.md)
- [Identity arithmetic function](identity-arithmetic-function.md)
- [Identity for Dirichlet convolution](identity-for-dirichlet-convolution.md)
- [Möbius divisor-sum identity](mobius-divisor-sum-identity.md)
- [Möbius function](mobius-function.md)
- [Möbius inversion formula](mobius-inversion-formula.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-25/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/11h/a/solution.md)
