# Totient divisor-sum identity

↑ **Parent:** [Euler totient function](euler-totient-function.md)

The [divisor sum](divisor-sum.md) of [Euler's totient function](euler-totient-function.md) is the [identity arithmetic function](identity-arithmetic-function.md):

$$
\sum_{d\mid n}\varphi(d)=n,\qquad n>0.
$$

Equivalently, $\varphi*\mathbf1=\operatorname{id}$ under [Dirichlet convolution](dirichlet-convolution.md), with $\mathbf1$ the [constant-one arithmetic function](constant-one-arithmetic-function.md). [Darij Grinberg, MIT 18.781 lecture notes, Propositions 2.4.4 and 2.4.5](https://darijgrinberg.gitlab.io/floor.pdf)

To see why, group the [integers](integer-split.md) $j=1,\ldots,n$ by $h=\gcd(j,n)$. Each $h$ is a positive [integer divisor](divisor.md) of $n$. Within its group, $j=ha$ with $1\leq a\leq n/h$ and $\gcd(a,n/h)=1$, by the [scaling identity for greatest common divisors](scaling-identity-for-greatest-common-divisors.md). Dividing by $h$ gives a [bijection](bijection.md) with the [integers](integer-split.md) counted by $\varphi(n/h)$. The groups form a [partition of a set](partition-of-a-set.md), so

$$
n=\sum_{h\mid n}\varphi(n/h)=\sum_{d\mid n}\varphi(d).
$$

For $n=12$, the groups with [greatest common divisor](greatest-common-divisor.md) $h=1,2,3,4,6,12$ are respectively $\{1,5,7,11\},\{2,10\},\{3,9\},\{4,8\},\{6\},\{12\}$. Their sizes are $4,2,2,2,1,1$, totaling $12$. [Möbius inversion](mobius-inversion-formula.md) reverses this [divisor sum](divisor-sum.md) to recover [Euler's totient function](euler-totient-function.md) from $g(n)=n$.

## ↑ Ancestors (5)

1. [Euler totient function](euler-totient-function.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Möbius inversion formula](mobius-inversion-formula.md)
