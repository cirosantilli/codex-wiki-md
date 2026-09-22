<h1 id="wilson-s-theorem">Wilson's theorem</h1>

↑ **Parent:** [Modular arithmetic](modular-arithmetic-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wilson's_theorem)

For an [integer](integer-split.md) $n>1$, [Wilson's theorem](wilson-s-theorem.md) characterizes [prime numbers](prime-number-split.md) by a [factorial](factorial.md):

$$
n\text{ is prime}\quad\Longleftrightarrow\quad(n-1)!\equiv-1\pmod n.
$$

The right side is an [integer congruence](integer-congruence.md), so the least nonnegative [remainder](remainder.md) is $n-1$. For example, $4!=24\equiv4\pmod5$ certifies that five is a [prime number](prime-number-split.md), whereas $5!=120\equiv0\pmod6$ rules out six. [Wilson's Theorem and Fermat's Theorem by Bruce Ikenaga](wilson-s-theorem-and-fermat-s-theorem-by-bruce-ikenaga.md)

<a id="image-factorial-residues-distinguish-primes-from-composites-with-inverse-pairs-explaining-the-prime-case"></a>
![](wilson-factorial-residue-primality.png)

**[Figure 2](#image-factorial-residues-distinguish-primes-from-composites-with-inverse-pairs-explaining-the-prime-case). Factorial residues distinguish primes from composites, with inverse pairs explaining the prime case**.

For an odd [prime number](prime-number-split.md) $p$, each nonzero [congruence class](congruence-class.md) has a unique [modular multiplicative inverse](modular-multiplicative-inverse.md). Pair each class with its inverse: each distinct pair contributes one. A class is its own inverse exactly when $a^2\equiv1\pmod p$; since $p\mid(a-1)(a+1)$, [Euclid's lemma](euclid-s-lemma.md) leaves only $a\equiv\pm1$. Their product is $-1$. The [prime number](prime-number-split.md) two needs a separate check: $1!\equiv-1\pmod2$. Conversely, a proper [divisor](divisor.md) $1<d<n$ divides both $n$ and $(n-1)!$, so the displayed [integer congruence](integer-congruence.md) would force $d\mid1$, a contradiction. [Wilson's Theorem and Fermat's Theorem by Bruce Ikenaga](wilson-s-theorem-and-fermat-s-theorem-by-bruce-ikenaga.md)

The [composite numbers](composite-number.md) have an even sharper pattern: $(n-1)!\equiv0\pmod n$ for every [composite number](composite-number.md) $n>4$, but $3!=6\equiv2\pmod4$. To check the zero claim, write $n=ab$ with $1<a\leq b<n$. If $a<b$, both occur as different factors in the [factorial](factorial.md). If $a=b\geq3$, the different factors $a$ and $2a$ both occur since $2a<a^2=n$, and their product is divisible by $n$. The only excluded case is $a=b=2$. Thus four is an exception to the zero pattern, but still fails [Wilson's theorem](wilson-s-theorem.md): its required [remainder](remainder.md) would be three.

This is an exact [primality testing](primality-testing.md) criterion, but direct evaluation is expensive: even reducing modulo $n$ after every multiplication still takes a number of multiplications proportional to $n$, which grows exponentially with the number of [binary digits](binary-digit.md) of $n$. The problem is not merely storing a huge [factorial](factorial.md). The more useful role of [Wilson's theorem](wilson-s-theorem.md) is simplifying [factorial](factorial.md) expressions in [modular arithmetic](modular-arithmetic-split.md). For instance, if $p>2$ is a [prime number](prime-number-split.md), then $(p-1)(p-2)!\equiv-1\pmod p$ gives $(p-2)!\equiv1\pmod p$ by a [modular multiplicative inverse](modular-multiplicative-inverse.md).

**Table of contents**

- [Wilson factorial congruence modulo a triangular number](wilson-factorial-congruence-modulo-a-triangular-number.md)
- [Odd-residue squared product modulo a prime](odd-residue-squared-product-modulo-a-prime.md)
- [Complementary factorial congruence](complementary-factorial-congruence.md)

## ↑ Ancestors (5)

1. [Modular arithmetic](modular-arithmetic-split.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4/5e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4/5e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4/7e/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-4/7b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-3/11h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-4/11f/i/solution.md)
- [Wilson factorial congruence modulo a triangular number](wilson-factorial-congruence-modulo-a-triangular-number.md)
- [Wilson's theorem](wilson-s-theorem.md)
