<h1 id="euler-s-criterion">Euler's criterion</h1>

↑ **Parent:** [Legendre symbol](legendre-symbol.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler's_criterion)

For an [odd prime](odd-prime.md) $p$ and $p\nmid a$, Euler's criterion identifies the [Legendre symbol](legendre-symbol.md) by [modular exponentiation](modular-exponentiation.md):

$$
a^{(p-1)/2}\equiv\left(\frac ap\right)\pmod p.
$$

Thus a [quadratic residue](quadratic-residue-split.md) gives one and a [quadratic nonresidue](quadratic-nonresidue.md) gives minus one, represented by $p-1$ if a nonnegative [remainder](remainder.md) is used. The formula also holds when $p\mid a$, because $(p-1)/2>0$ and both sides are zero modulo $p$.[Ben Lynn, Quadratic Residues, Euler's Criterion and The Legendre Symbol: exponent test and the zero value](quadratic-residues-by-ben-lynn.md)

For example, modulo seven the exponent is three: $2^3\equiv1$ confirms that two is a [quadratic residue](quadratic-residue-split.md), while $3^3\equiv6\equiv-1$ confirms that three is a [quadratic nonresidue](quadratic-nonresidue.md). Modulo eleven the exponent is five, and $2^5=32\equiv10\equiv-1$ confirms that two is a [quadratic nonresidue](quadratic-nonresidue.md). The test answers whether a [square root](square-root.md) exists; it does not itself return the roots $3,4$ of $x^2\equiv2\pmod7$.

A short proof needs only [Fermat's little theorem](fermat-little-theorem.md) and the [root bound for a polynomial](lagrange-root-bound-over-a-field.md). Put $m=(p-1)/2$. If $a=x^2\ne0$ in the [prime field](prime-field.md), then $a^m=x^{p-1}=1$. There are already $m$ such [quadratic residues](quadratic-residue-split.md). The nonzero [polynomial](polynomial-split.md) $T^m-1$ has [polynomial degree](degree-of-a-polynomial.md) $m$, so it has no other [polynomial roots](root-of-a-polynomial.md). Finally, for every nonzero $a$, [Fermat's little theorem](fermat-little-theorem.md) gives $(a^m)^2=a^{p-1}=1$. Factoring $(a^m-1)(a^m+1)=0$ in the [field](field.md) shows $a^m\in\{1,-1\}$; every [quadratic nonresidue](quadratic-nonresidue.md) must take the remaining value $-1$. This proves the criterion without first finding a [primitive root](primitive-root-modulo-n.md).

For a larger original example, decide whether seven is a [quadratic residue](quadratic-residue-split.md) modulo the [prime number](prime-number-split.md) $101$. [Exponentiation by squaring](exponentiation-by-squaring.md) computes the required power without listing fifty squares:

$$
\begin{aligned}
7^2&\equiv49,&7^4&\equiv78,&7^8&\equiv24,\\
7^{16}&\equiv71,&7^{32}&\equiv92,\\
7^{50}&=7^{32}7^{16}7^2\equiv92\cdot71\cdot49\equiv-1\pmod{101}.
\end{aligned}
$$

Therefore $(7/101)=-1$ and $x^2\equiv7\pmod{101}$ has no solution. Each intermediate product is reduced modulo $101$, as in [modular exponentiation](modular-exponentiation.md). The advantage is that [exponentiation by squaring](exponentiation-by-squaring.md) uses a number of [multiplications](multiplication.md) proportional to the [binary digit](binary-digit.md) length of the exponent rather than testing every potential [square root](square-root.md).

The [odd prime](odd-prime.md) hypothesis is essential. For the composite modulus nine, $2^{(9-1)/2}=2^4\equiv7\pmod9$, which is neither one nor minus one. Although four is a nonzero square modulo nine, $4^4\equiv4\pmod9$, so even the square-to-one implication fails. The [Jacobi symbol](jacobi-symbol.md) and [Euler pseudoprime](euler-pseudoprime.md) discuss different questions for odd composite moduli; they do not make this a universal square test.

**Table of contents**

- [Primes congruent to five modulo eight from odd squares plus four](primes-congruent-to-five-modulo-eight-from-odd-squares-plus-four.md)

## ↑ Ancestors (6)

1. [Legendre symbol](legendre-symbol.md)
2. [Quadratic residue](quadratic-residue-split.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (17)

- [Multiplicativity of the Legendre symbol](multiplicativity-of-the-legendre-symbol.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-2/17b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-3/9f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1/17g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1/17g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/1f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/1g/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4/6e/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4/6e/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1/1h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/11h/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/1i/solution.md)
- [Pépin's test](pepin-s-test.md)
- [Quadratic residue](quadratic-residue-split.md)
- [Solovay-Strassen primality test](solovay-strassen-primality-test.md)
- [Stronger prime-divisor congruence for Fermat numbers](stronger-prime-divisor-congruence-for-fermat-numbers.md)
