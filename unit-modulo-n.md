# Unit modulo n

↑ **Parent:** [Modular congruence](modular-congruence.md)

For a positive [integer modulus](modulus-in-modular-arithmetic.md) $n$, a [residue class](residue-class.md) $[a]_n$ is a [unit](unit-in-a-ring.md) when it has a [modular multiplicative inverse](modular-multiplicative-inverse.md): some [integer](integer.md) $u$ satisfies $au\equiv1\pmod n$. Modulo twelve, the [units](unit-in-a-ring.md) are exactly

$$
[1]_{12},\quad[5]_{12},\quad[7]_{12},\quad[11]_{12}.
$$

In particular, five is its own [modular inverse](modular-multiplicative-inverse.md), since $5\cdot5=25\equiv1\pmod{12}$. Multiplying all twelve [residue classes](residue-class.md) by five gives a [permutation](permutation.md); multiplying the outputs by five recovers the inputs. By contrast, multiplying by six gives only zero and six, with six inputs for each output. It cannot be reversed.

<a id="image-multiplication-by-five-permutes-all-twelve-residue-classes-whereas-multiplication-by-six-merges-distinct-inputs"></a>
![](modular-multiplication-units-and-zero-divisors.png)

**[Figure 33](#image-multiplication-by-five-permutes-all-twelve-residue-classes-whereas-multiplication-by-six-merges-distinct-inputs). Multiplication by five permutes all twelve residue classes, whereas multiplication by six merges distinct inputs**.

In general, the exact criterion is

$$
[a]_n\text{ is a unit}\iff\gcd(a,n)=1.
$$

For the forward direction, $au-kn=1$ implies every common [divisor](divisor.md) of $a,n$ divides one. Conversely, if their [greatest common divisor](greatest-common-divisor.md) is one, [Bézout's identity](bezout-s-identity.md) supplies $ua+vn=1$, so $u$ is a [modular inverse](modular-multiplicative-inverse.md). The [extended Euclidean algorithm](extended-euclidean-algorithm.md) computes these coefficients. The [units](unit-in-a-ring.md) form the [unit group](unit-group.md) $(\mathbb Z/n\mathbb Z)^\times$ under [multiplication](multiplication.md). [Ankur Moitra, MIT 18.200, Lecture 15 (2024), pp. 3–4: inverses, coprimality and the unit group](https://ocw.mit.edu/courses/18-200-principles-of-discrete-applied-mathematics-spring-2024/mit18_200_s24_lec15.pdf)

[Multiplicative cancellation](multiplicative-cancellation-in-an-integral-domain.md) while keeping the same [integer modulus](modulus-in-modular-arithmetic.md) is valid for a [unit modulo n](unit-modulo-n.md): from $ca\equiv cb\pmod n$, multiply by a [modular inverse](modular-multiplicative-inverse.md) of $c$ to get $a\equiv b\pmod n$. A nonunit cannot be cancelled as a general rule. For example, $6\cdot0\equiv6\cdot2\pmod{12}$, yet $0\not\equiv2\pmod{12}$. Thus [division](division-mathematics.md) by six cannot undo this [multiplication](multiplication.md); solving a [linear congruence](linear-congruence.md) instead keeps track of all possible classes.

This distinction marks the boundary between [commutative rings](commutative-ring.md) and [fields](field.md). Modulo a [prime number](prime-number.md) $p>1$, every nonzero [residue class](residue-class.md) is a [unit](unit-in-a-ring.md), so $\mathbb Z/p\mathbb Z$ is a [finite field](finite-field.md). Modulo twelve it is a [commutative ring](commutative-ring.md) with [zero divisors](zero-divisor.md), and is not a [field](field.md). For $n=1$, the sole class satisfies $[0]_1=[1]_1$ and is a [unit](unit-in-a-ring.md); this one-element [zero ring](zero-ring.md) is not a [field](field.md). [Moitra, MIT 18.200, Lecture 15, pp. 8–9: the prime-modulus field criterion](https://ocw.mit.edu/courses/18-200-principles-of-discrete-applied-mathematics-spring-2024/mit18_200_s24_lec15.pdf)

## ↑ Ancestors (6)

1. [Modular congruence](modular-congruence.md)
2. [Modular arithmetic](modular-arithmetic.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Exponent reduction for units](exponent-reduction-for-units.md)
- [Multiplication by a unit permutes reduced residues](multiplication-by-a-unit-permutes-reduced-residues.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4/5d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4/5d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-4/6e/c/solution.md)
- [Reduced residue system](reduced-residue-system.md)
- [Residue class](residue-class.md)
- [Unit modulo n](unit-modulo-n.md)
