# Residue class

↑ **Parent:** [Modular congruence](modular-congruence.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Residue_class)

For a positive [integer modulus](modulus-in-modular-arithmetic.md) $m$, the residue class of an [integer](integer-split.md) $a$ is the [equivalence class](equivalence-class.md)

$$
[a]_m=\{a+km:k\in\mathbb Z\}=\{b\in\mathbb Z:b\equiv a\pmod m\}.
$$

It contains all [integers](integer-split.md) in the same position of the repeating cycle. For example,

$$
[-1]_{12}=[11]_{12}=\{\ldots,-13,-1,11,23,35,\ldots\}.
$$

The [residue class](residue-class.md) is this whole infinite collection; its canonical representative is the [least nonnegative residue](least-nonnegative-residue.md). [Euclidean division](euclidean-division.md) gives exactly one such representative in $0,1,\ldots,m-1$, so there are exactly $m$ [residue classes](residue-class.md). When $m=1$, there is just one, $[0]_1=\mathbb Z$.

Define [addition](addition.md) and [multiplication](multiplication.md) of [residue classes](residue-class.md) by

$$
[a]_m+[b]_m=[a+b]_m,\qquad [a]_m[b]_m=[ab]_m.
$$

These definitions must give the same answer whichever [integers](integer-split.md) represent the classes. If $a'\equiv a$ and $b'\equiv b$ modulo $m$, then

$$
(a'+b')-(a+b)=(a'-a)+(b'-b),\qquad a'b'-ab=b'(a'-a)+a(b'-b).
$$

Both differences are divisible by $m$, proving that the operations are well-defined. For example, $[9]_{12}+[5]_{12}=[2]_{12}$ and $[9]_{12}[5]_{12}=[9]_{12}$, since $45=3\cdot12+9$. Replacing nine by $-3$ gives the same answers with smaller intermediate [integers](integer-split.md).

With these operations the [residue classes](residue-class.md) form the finite [commutative ring](commutative-ring.md) $\mathbb Z/m\mathbb Z$, a [quotient ring](quotient-ring.md). It need not be a [field](field.md): $[6]_{12}[2]_{12}=[0]_{12}$ although neither factor is the zero class. These [zero divisors](zero-divisor.md) explain why [division](division-mathematics.md) requires a [unit modulo n](unit-modulo-n.md). Reducing after each [multiplication](multiplication.md) is especially useful in [modular exponentiation](modular-exponentiation.md), where the unreduced powers can become enormous.

## ↑ Ancestors (6)

1. [Modular congruence](modular-congruence.md)
2. [Modular arithmetic](modular-arithmetic-split.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (65)

- [Batch modular inversion](batch-modular-inversion.md)
- [Bounded exceptional primes for least quadratic nonresidues](bounded-exceptional-primes-for-least-quadratic-nonresidues.md)
- [Carmichael number](carmichael-number.md)
- [Character sum of a Dirichlet character](character-sum-of-a-dirichlet-character.md)
- [Commutative ring](commutative-ring.md)
- [Complementary factorial congruence](complementary-factorial-congruence.md)
- [Cyclic convolution](cyclic-convolution.md)
- [Direct product of groups](direct-product-of-groups.md)
- [Equivalence class](equivalence-class.md)
- [Fermat little theorem](fermat-little-theorem.md)
- [Fermat witness](fermat-witness.md)
- [Infinite pigeonhole principle](infinite-pigeonhole-principle.md)
- [Integers with all prime factors congruent to one modulo four](integers-with-all-prime-factors-congruent-to-one-modulo-four.md)
- [Internal direct product theorem](internal-direct-product-theorem.md)
- [Large sieve](large-sieve.md)
- [Least quadratic nonresidue](least-quadratic-nonresidue.md)
- [Modular congruence](modular-congruence.md)
- [Nonzero residue permutation](nonzero-residue-permutation.md)
- [One-equation partition regularity over odd integers](one-equation-partition-regularity-over-odd-integers.md)
- [Passing-base fraction for the Fermat test](passing-base-fraction-for-the-fermat-test.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4/5e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4/7e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-25/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-4/1c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-4/6c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-4/6c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-22/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-28/7/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-31/5/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-28/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-4/6d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-4/6d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-4/6d/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1/12f/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-9/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-10/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-10/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-23/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-23/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-23/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4/6e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4/6e/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4/6e/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4/1d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4/5d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4/5d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4/10g/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4/3g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-137/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-4/5e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/1h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/1h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-150/1/c/solution.md)
- [Pigeonhole principle](pigeonhole-principle.md)
- [Profinite topology on the integers is not compact](profinite-topology-on-the-integers-is-not-compact.md)
- [Quotient set](quotient-set.md)
- [Reduced residue system](reduced-residue-system.md)
- [Residue class](residue-class.md)
- [Strong induction with four starting cases](strong-induction-with-four-starting-cases.md)
- [Three power summands over a large prime field](three-power-summands-over-a-large-prime-field.md)
- [Twin-prime upper bound from a quadratic sieve](twin-prime-upper-bound-from-a-quadratic-sieve.md)
- [Unit modulo n](unit-modulo-n.md)
- [Wheel factorization](wheel-factorization.md)
- [Zero-residue constraint for idempotent ultrafilters](zero-residue-constraint-for-idempotent-ultrafilters.md)
