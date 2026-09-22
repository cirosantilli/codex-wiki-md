# Least common multiple

↑ **Parent:** [Divisibility](divisibility-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Least_common_multiple)

For [positive integers](positive-integer.md) $a,b$, their least common multiple is the **smallest positive [integer](integer-split.md) that is an [integer multiple](integer-multiple.md) of both**. Write it as $\operatorname{lcm}(a,b)$. A positive common [integer multiple](integer-multiple.md) always exists, since $ab$ is one, but it can be larger than necessary.

For example, the positive [integer multiples](integer-multiple.md) of $12$ begin $12,24,36,48,60,72$, while those of $18$ begin $18,36,54,72$. Their first positive coincidence is $36$, so $\operatorname{lcm}(12,18)=36$. Both also divide zero, but the word positive excludes zero from this minimum.

Suppose two events happen every twelve and eighteen days, and both happen at day $t=0$. Their next meeting is at day $36$, after three twelve-day intervals and two eighteen-day intervals. Through day $72$, their common event times are $0,36,72$.

<a id="image-events-every-12-and-18-days-starting-together-meet-again-every-36-days"></a>
![](least-common-multiple-periods.png)

**[Figure 2](#image-events-every-12-and-18-days-starting-together-meet-again-every-36-days). Events every 12 and 18 days, starting together, meet again every 36 days**. Each row marks the nonnegative [integer multiples](integer-multiple.md) of its interval from zero through 72. The highlighted columns $0,36,72$ are shared; 36 is the first positive one and hence the [least common multiple](least-common-multiple.md).

The [prime factorization](fundamental-theorem-of-arithmetic.md) explains why this coincidence occurs. For the [integers](integer-split.md) $12$ and $18$,

$$
12=2^2\cdot3,\qquad18=2\cdot3^2,\qquad
\operatorname{lcm}(12,18)=2^{\max(2,1)}3^{\max(1,2)}=36.
$$

A common [integer multiple](integer-multiple.md) must contain at least the [prime valuations](prime-valuation.md) required by each input. Taking the larger [prime valuation](prime-valuation.md) at each [prime number](prime-number-split.md) meets both requirements with no extra factors. The [greatest common divisor](greatest-common-divisor.md) uses the smaller [prime valuations](prime-valuation.md) instead. This is the same coordinate comparison developed under [prime factorization](fundamental-theorem-of-arithmetic.md), applied in opposite directions.

<a id="image-for-12-and-18-smaller-prime-valuations-give-greatest-common-divisor-6-and-larger-ones-give-least-common-multiple-36"></a>
![](gcd-lcm-prime-exponents.png)

**[Figure 3](#image-for-12-and-18-smaller-prime-valuations-give-greatest-common-divisor-6-and-larger-ones-give-least-common-multiple-36). For 12 and 18, smaller prime valuations give greatest common divisor 6 and larger ones give least common multiple 36**. Bars show the exponents of the [prime numbers](prime-number-split.md) two and three in $12$, $18$, $6$ and $36$. The table makes the minimum and maximum in each column explicit.

For any [positive integers](positive-integer.md) $a,b$, the [prime valuations](prime-valuation.md) give

$$
\gcd(a,b)\operatorname{lcm}(a,b)=ab,\qquad
\operatorname{lcm}(a,b)=\frac{ab}{\gcd(a,b)}.
$$

The proof outline is one observation at each [prime number](prime-number-split.md): $\min(r,s)+\max(r,s)=r+s$. Hence the two sides have identical [prime factorizations](fundamental-theorem-of-arithmetic.md). Numerically, $6\cdot36=12\cdot18=216$. This also gives a calculation using the [Euclidean algorithm](euclidean-algorithm.md) for the [greatest common divisor](greatest-common-divisor.md), without first finding the [prime factors](prime-factor.md) of both inputs.

Every positive common [integer multiple](integer-multiple.md) is an [integer multiple](integer-multiple.md) of the [least common multiple](least-common-multiple.md), because its [prime valuations](prime-valuation.md) must be at least the larger input [prime valuations](prime-valuation.md). Including negatives and zero, the common [integer multiples](integer-multiple.md) of $12$ and $18$ are exactly $36k$ for [integers](integer-split.md) $k$. For more than two [positive integers](positive-integer.md), the same definition and rule of taking the largest [prime valuations](prime-valuation.md) apply; one may also combine inputs successively. For example, $\operatorname{lcm}(12,18,20)=\operatorname{lcm}(36,20)=180$.

For nonzero signed [integers](integer-split.md), take [absolute values](absolute-value.md): $\operatorname{lcm}(-12,18)=36$. We extend the definition to zero by the convention $\operatorname{lcm}(a,0)=0$, since zero is then the only common [integer multiple](integer-multiple.md); this is an extension, not a positive minimum. In particular $\operatorname{lcm}(0,0)=0$ must be handled separately from the displayed [quotient](quotient.md), which would involve [division](division-mathematics.md) by zero.

The [least common multiple](least-common-multiple.md) is useful for combining [fractions](fraction.md) with the smallest positive shared [denominator](denominator.md). For example,

$$
\frac1{12}+\frac1{18}=\frac3{36}+\frac2{36}=\frac5{36}.
$$

Its scheduling interpretation requires care about starting times. If the events start at [integer](integer-split.md) days $r$ and $s$, a common time must satisfy the [integer congruences](integer-congruence.md) $t\equiv r\pmod{12}$ and $t\equiv s\pmod{18}$. The [Chinese remainder theorem for noncoprime moduli](chinese-remainder-theorem-for-noncoprime-moduli.md) says a solution exists exactly when $6\mid(r-s)$. If it exists, solutions form one [congruence class](congruence-class.md) modulo $36$, but the first meeting need not be day $36$. With starts $r=0,s=6$, the first meeting is day $24$ and subsequent meetings are $60,96,\ldots$; with $r=0,s=1$, they never meet. The beauty of the [least common multiple](least-common-multiple.md) is the exact shared spacing, while the [integer congruences](integer-congruence.md) determine whether and where the spacing begins.

Book VII, Proposition 34 of [Euclid's Elements](euclid-s-elements.md) constructs the [least common multiple](least-common-multiple.md) of two numbers, and Proposition 36 extends the construction to three by first combining two of them. In modern notation this is $\operatorname{lcm}(a,b,c)=\operatorname{lcm}(\operatorname{lcm}(a,b),c)$. These are specific ancient treatments of the construction, rather than a claim about its first discovery. [Euclid, Elements VII.34, T. L. Heath translation: two numbers](https://geometor.github.io/euclid/heath/VII/34/index.html) [Euclid, Elements VII.36, T. L. Heath translation: three numbers](https://geometor.github.io/euclid/heath/VII/36/index.html)

## ↑ Ancestors (5)

1. [Divisibility](divisibility-split.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (38)

- [Carmichael function](carmichael-function.md)
- [Chinese remainder theorem](chinese-remainder-theorem.md)
- [Chinese remainder theorem for noncoprime moduli](chinese-remainder-theorem-for-noncoprime-moduli.md)
- [Counting cyclic subgroups by their generators](counting-cyclic-subgroups-by-their-generators.md)
- [Cyclicity of a product of two finite cyclic groups](cyclicity-of-a-product-of-two-finite-cyclic-groups.md)
- [Disjoint permutation cycles](disjoint-permutation-cycles.md)
- [Divisor lattice](divisor-lattice.md)
- [Fundamental theorem of arithmetic](fundamental-theorem-of-arithmetic.md)
- [Greatest common divisor](greatest-common-divisor.md)
- [Homomorphism from a finite cyclic group](homomorphism-from-a-finite-cyclic-group.md)
- [Integer multiple](integer-multiple.md)
- [Least common multiple](least-common-multiple.md)
- [Order of a direct-product element](order-of-a-direct-product-element.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-28/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-1/1h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-3/1h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-3/1d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-3/5d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-3/6e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-4/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-7/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-3/5d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-4/5d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-29/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-3/2d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-61/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-3/2d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-27/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-3/5d/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-104/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-130/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-324/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2/9/b/solution.md)
- [Prime number](prime-number-split.md)
- [Reciprocal partition regularity](reciprocal-partition-regularity.md)
- [Second Chebyshev function](second-chebyshev-function.md)
- [Three to the distinct-prime-factor count](three-to-the-distinct-prime-factor-count.md)
- [Uniform period criterion for pointwise periodic maps](uniform-period-criterion-for-pointwise-periodic-maps.md)
