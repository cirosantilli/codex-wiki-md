# Prime omega function

↑ **Parent:** [Arithmetic function](arithmetic-function-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prime_omega_function)

The [prime omega function](prime-omega-function.md) $\omega(n)$ counts the distinct [prime factors](prime-factor.md) of a [positive integer](positive-integer.md) $n$, so it is the [cardinality](cardinality.md) of the [prime support of an integer](prime-support-of-an-integer.md) $P(n)$. For a [prime factorization](fundamental-theorem-of-arithmetic.md) with distinct [prime numbers](prime-number-split.md) $p_1,\ldots,p_r$ and positive exponents,

$$
n=p_1^{a_1}\cdots p_r^{a_r}\quad\Longrightarrow\quad
\omega(n)=r=\sum_{p\mid n}1.
$$

At $n=1$ there are no [prime factors](prime-factor.md), so the [empty sum](empty-sum.md) gives $\omega(1)=0$. The [total number of prime factors](total-number-of-prime-factors.md) instead gives $\Omega(n)=\sum_i a_i$. [Darij Grinberg, MIT 18.781, Floor and arithmetic functions, Definition 2.1.2: distinct and repeated prime factors](https://darijgrinberg.gitlab.io/floor.pdf)

For $72=2^3\cdot3^2$, the [prime support of an integer](prime-support-of-an-integer.md) is $\{2,3\}$ and $\omega(72)=2$. The comparison examples give $\omega(30)=3$, $\omega(32)=1$ and $\omega(36)=2$. Raising an existing [prime factor](prime-factor.md) to a higher power does not affect the [prime omega function](prime-omega-function.md): $\omega(p^k)=1$ for a [prime number](prime-number-split.md) $p$ and $k\ge1$. Thus the [prime omega function](prime-omega-function.md) is a [strongly additive arithmetic function](strongly-additive-arithmetic-function.md), with

$$
\omega(ab)=\omega(a)+\omega(b)\quad\text{if }\gcd(a,b)=1.
$$

The reason is that [coprime integers](coprime-integers.md) have disjoint [prime supports of an integer](prime-support-of-an-integer.md). For arbitrary [positive integers](positive-integer.md), their [prime support of an integer](prime-support-of-an-integer.md) combines by [set union](set-union.md), and the shared [prime factors](prime-factor.md) are exactly those of the [greatest common divisor](greatest-common-divisor.md). Counting this [set union](set-union.md) gives the more general identity

$$
\omega(ab)=\omega(a)+\omega(b)-\omega(\gcd(a,b)).
$$

For $a=12$, $b=18$, both [prime supports of an integer](prime-support-of-an-integer.md) are $\{2,3\}$ and $\gcd(a,b)=6$, so $\omega(216)=2+2-2=2$. In particular $\omega(4)=1\ne2=\omega(2)+\omega(2)$: the [prime omega function](prime-omega-function.md) is not a [completely additive arithmetic function](completely-additive-arithmetic-function.md).

The [prime omega function](prime-omega-function.md) is useful for counting choices involving distinct [prime factors](prime-factor.md). Every [squarefree divisor](squarefree-divisor.md) of $n$ chooses a [subset](subset.md) of its [prime support of an integer](prime-support-of-an-integer.md), so there are $2^{\omega(n)}$ [squarefree divisors](squarefree-divisor.md). For $72$, this gives $2^2=4$, namely $1,2,3,6$. Also $\omega(\operatorname{rad}(n))=\omega(n)$, because the [radical of an integer](radical-of-an-integer.md) keeps exactly that [prime support of an integer](prime-support-of-an-integer.md). The [total number of prime factors](total-number-of-prime-factors.md) records what this count discards, and the two counts agree exactly on [squarefree integers](square-free-integer.md).

**Table of contents**

- [Three to the distinct-prime-factor count](three-to-the-distinct-prime-factor-count.md)
  - [Summatory bound for three to the prime omega](summatory-bound-for-three-to-the-prime-omega.md)
  - [Log-weighted convolution bound for three to the prime omega](log-weighted-convolution-bound-for-three-to-the-prime-omega.md)

## ↑ Ancestors (5)

1. [Arithmetic function](arithmetic-function-split.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Erdős-Kac theorem](erdos-kac-theorem.md)
- [Multiplication table bound from distinct prime factors](multiplication-table-bound-from-distinct-prime-factors.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-27/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-27/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-124/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-124/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-124/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-124/5/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-150/1/b/solution.md)
- [Prime omega function](prime-omega-function.md)
- [Prime support of an integer](prime-support-of-an-integer.md)
- [Radical of an integer](radical-of-an-integer.md)
- [Strongly additive arithmetic function](strongly-additive-arithmetic-function.md)
- [Total number of prime factors](total-number-of-prime-factors.md)
- [Turán normal-order theorem for distinct prime divisors](turan-normal-order-theorem-for-distinct-prime-divisors.md)
