# Fermat little theorem

↑ **Parent:** [Number theory](number-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fermat's_little_theorem)

For a [prime number](prime-number-split.md) $p$ and an [integer](integer-split.md) $a$ not divisible by $p$, [Fermat's little theorem](fermat-little-theorem.md) states the [modular congruence](modular-congruence.md)

$$
a^{p-1}\equiv1\pmod p\qquad(p\nmid a).
$$

Equivalently, for every [integer](integer-split.md) $a$, including $a<0$ and multiples of $p$,

$$
a^p\equiv a\pmod p.
$$

The first formulation follows from the second by multiplying by a [modular multiplicative inverse](modular-multiplicative-inverse.md) of $a$. Conversely, multiply the first by $a$ when $p\nmid a$; when $p\mid a$, both sides of the second are zero modulo $p$. The [divisibility](divisibility-split.md) condition in the first formulation is essential.[p. 1, Theorem 1.1 and the equivalence of nonzero and coprime classes for a prime modulus](euler%E2%80%99s-theorem-by-keith-conrad.md)

For $p=7$, $3^6=729=7\cdot104+1$, so $3^6\equiv1\pmod7$ and $3^7\equiv3\pmod7$. Also $(-2)^6=64\equiv1\pmod7$, while $7^6\equiv0\pmod7$: a zero [residue class](residue-class.md) cannot satisfy the first formulation. It does satisfy $7^7\equiv7\equiv0\pmod7$. A failure at a zero [residue class](residue-class.md) therefore says nothing against a candidate's being a [prime number](prime-number-split.md).

The [prime number](prime-number-split.md) $p=2$ is included. Its only nonzero [residue class](residue-class.md) is one: every odd [integer](integer-split.md) $a$ satisfies $a^{2-1}=a\equiv1\pmod2$. Every [integer](integer-split.md) also satisfies $a^2\equiv a\pmod2$, because $a(a-1)$ is even. Testing the first formulation with an even [integer](integer-split.md) would violate its hypothesis.

The useful surprise is that every nonzero [residue class](residue-class.md) returns to one at the same [exponent](exponent.md) $p-1$, although its shortest return can be earlier. This gives [exponent reduction for units](exponent-reduction-for-units.md): for a [nonnegative integer](natural-number.md) $k$, $a^k\equiv a^{k\bmod(p-1)}\pmod p$ when $p\nmid a$. It also computes a [modular multiplicative inverse](modular-multiplicative-inverse.md) as $a^{p-2}$ modulo $p$, including $p=2$. [Repeated squaring](exponentiation-by-squaring.md) makes these [modular exponentiations](modular-exponentiation.md) practical.

In [group theory](group-theory-split.md), the nonzero [residue classes](residue-class.md) form the [multiplicative group of integers modulo n](multiplicative-group-of-integers-modulo-n.md) with $n=p$, of [group order](order-of-a-finite-group.md) $p-1$. [Lagrange's theorem](lagrange-s-theorem.md) says that the [multiplicative order](multiplicative-order.md) of $a$ divides $p-1$, giving the guaranteed return. [Euler's theorem](euler-s-theorem.md) extends this to a general [integer modulus](modulus-in-modular-arithmetic.md) $n$, using the [units](unit-in-a-ring.md) and [Euler's totient function](euler-totient-function.md) $\varphi(n)$; the [Carmichael function](carmichael-function.md) gives the least common return [exponent](exponent.md) for all [units](unit-in-a-ring.md). A nonzero [residue class](residue-class.md) modulo a [composite number](composite-number.md) need not be a [unit](unit-in-a-ring.md).

[Leonhard Euler](leonhard-euler.md)'s paper presented in 1732 and published in 1738 states a historical formulation: Theorem 1 says that powers with [exponent](exponent.md) $n-1$ leave zero or one upon division by a [prime number](prime-number-split.md) $n$. The preceding discussion states the difference-of-powers version and explicitly says that he does not have its proof.[English translation, p. 1 publication note; p. 2 paragraph before footnote 3; p. 3, Theorem 1](observations-on-a-certain-theorem-of-fermat-and-on-others-concerning-prime-numbers-by-leonhard-euler.md)

**Table of contents**

- [Nonzero residue permutation](nonzero-residue-permutation.md)
- [Fermat witness](fermat-witness.md)
- [Fermat test example](fermat-test-example.md)

## ↑ Ancestors (4)

1. [Number theory](number-theory-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Fermat primality test](fermat-primality-test.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-4/6c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-4/6e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-4/1e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4/1e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4/6e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-4/2e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/9h/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-4/1e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-104/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/11g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/11g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ia/paper-4/1e/solution.md)
- [Repdigit](repdigit.md)
