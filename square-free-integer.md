# Square-free integer

↑ **Parent:** [Integer](integer-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Square-free_integer)

A [positive integer](positive-integer.md) $n$ is **square-free** when no [square number](square-number.md) greater than one is a [divisor](divisor.md) of $n$. It suffices to exclude squares of [prime numbers](prime-number-split.md); equivalently, every [prime valuation](prime-valuation.md) is zero or one:

$$
n\text{ is square-free}\quad\Longleftrightarrow\quad
p^2\nmid n\text{ for every prime }p
\quad\Longleftrightarrow\quad v_p(n)\in\{0,1\}\text{ for every prime }p.
$$

Thus the [prime factorization](fundamental-theorem-of-arithmetic.md) of a [square-free integer](square-free-integer.md) is a [product](product-of-numbers.md) of distinct [prime factors](prime-factor.md), with no repetitions. One is included: its [prime factorization](fundamental-theorem-of-arithmetic.md) is an [empty product](empty-product.md) and all its [prime valuations](prime-valuation.md) are zero. These equivalent tests are stated in Grinberg's notes. [Darij Grinberg, MIT 18.781, Floor and arithmetic functions, Definition 2.1.2 and footnote 6](https://darijgrinberg.gitlab.io/floor.pdf)

For signed [integers](integer-split.md), extend the definition by requiring $|n|$ to be a [square-free integer](square-free-integer.md), where $|n|$ denotes [absolute value](absolute-value.md). Hence $-30$ and both $1,-1$ qualify. Zero does not: every [prime number](prime-number-split.md) has its square as a [divisor](divisor.md) of zero. The [Möbius function](mobius-function.md) and [radical of an integer](radical-of-an-integer.md) below use their existing [positive integer](positive-integer.md) domains, so apply them to $|n|$ when handling a negative [integer](integer-split.md).

For example, $30=2\cdot3\cdot5$ is a [square-free integer](square-free-integer.md), whereas $12=2^2\cdot3$ is not, because $4\mid12$ and $v_2(12)=2$. Being a [composite number](composite-number.md) causes no problem: $6,10,15$ are all [square-free integers](square-free-integer.md). A [square-free integer](square-free-integer.md) need not be [coprime](coprime-integers.md) to another [integer](integer-split.md): $6$ and $10$ are both [square-free integers](square-free-integer.md) but have [greatest common divisor](greatest-common-divisor.md) two. In fact the only signed [integers](integer-split.md) [coprime](coprime-integers.md) to every [integer](integer-split.md) are $1,-1$, since $\gcd(n,n)=|n|$.

<a id="image-exact-square-free-integer-classification-of-the-integers-from-one-to-sixty"></a>
![](coprime-squarefree-integers-square-sieve.png)

**[Figure 5](#image-exact-square-free-integer-classification-of-the-integers-from-one-to-sixty). Exact square-free integer classification of the integers from one to sixty**. Green cells are [square-free integers](square-free-integer.md); each red cell displays a [prime number](prime-number-split.md) square that divides its label, choosing the smallest such [prime number](prime-number-split.md). Only $4,9,25,49$ need testing in this range. There are $37$ green cells. This original finite arithmetic diagram is an exact enumeration, not a measurement or an assertion about a limiting frequency.

For [positive integers](positive-integer.md) $a,b$, the useful [product](product-of-numbers.md) criterion is

$$
ab\text{ is square-free}\quad\Longleftrightarrow\quad
a,b\text{ are square-free and }\gcd(a,b)=1.
$$

The proof outline is just [addition](addition.md) of [prime valuations](prime-valuation.md): $v_p(ab)=v_p(a)+v_p(b)$ can stay at most one only if neither input repeats a [prime factor](prime-factor.md) and no [prime factor](prime-factor.md) occurs in both. Thus $6\cdot5=30$ is a [square-free integer](square-free-integer.md), but $6\cdot10=60$ is not. An equivalent characterization is that **every** factorization $n=ab$ into [positive integers](positive-integer.md) has [coprime](coprime-integers.md) factors. If $p^2\mid n$, the factorization $n=p(n/p)$ supplies two factors sharing $p$; conversely, a shared [prime factor](prime-factor.md) forces its square to divide $n$. For $30$, the unordered factor pairs $(1,30),(2,15),(3,10),(5,6)$ all have [greatest common divisor](greatest-common-divisor.md) one; for $12$, the pair $(2,6)$ fails.

Two existing [arithmetic functions](arithmetic-function-split.md) turn the definition into practical tests:

$$
\operatorname{rad}(n)=n\quad\Longleftrightarrow\quad n\text{ is square-free},\qquad
\mu(n)^2=\begin{cases}1&n\text{ is square-free},\\0&\text{otherwise},\end{cases}\qquad n>0.
$$

The [radical of an integer](radical-of-an-integer.md) keeps one copy of each [prime factor](prime-factor.md), so it changes precisely the [integers](integer-split.md) with a repeated [prime factor](prime-factor.md). Its definition is given in Evertse's exercise sheet. [Jan-Hendrik Evertse, Diophantine approximation, Homework IV, Exercise 20](https://pub.math.leidenuniv.nl/~evertsejh/dio12-ex4.pdf) The [Möbius function](mobius-function.md) assigns $(-1)^r$ to a [square-free integer](square-free-integer.md) with $r$ distinct [prime factors](prime-factor.md) and zero otherwise; squaring forgets the sign. Consequently $\sum_{n=1}^{60}\mu(n)^2=37$ counts exactly the green cells. This connects a restriction on repeated [prime factors](prime-factor.md) with weighted counting and [inclusion-exclusion](inclusion-exclusion-principle.md). [Darij Grinberg, MIT 18.781, Definition 2.1.2: the Möbius function](https://darijgrinberg.gitlab.io/floor.pdf)

**Table of contents**

- [Squarefree part](squarefree-part.md)
- [Squarefree counting function](squarefree-counting-function.md)

## ↑ Ancestors (5)

1. [Integer](integer-split.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (20)

- [Coprime integers](coprime-integers.md)
- [Integral basis of a cubefree pure cubic field](integral-basis-of-a-cubefree-pure-cubic-field.md)
- [Integral basis of a nonexceptional pure cubic field](integral-basis-of-a-nonexceptional-pure-cubic-field.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-28/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-27/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-28/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-125/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4/19h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-125/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/11g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/20g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2/20h/b/solution.md)
- [Pure cubic number field](pure-cubic-number-field.md)
- [Quadratic field](quadratic-field.md)
- [Rational group with square-free denominators](rational-group-with-square-free-denominators.md)
- [Rational halving quotient bound from root size](rational-halving-quotient-bound-from-root-size.md)
- [Ring of integers of a quadratic field](ring-of-integers-of-a-quadratic-field.md)
- [Square-free integer](square-free-integer.md)
- [Squarefree counting function](squarefree-counting-function.md)
