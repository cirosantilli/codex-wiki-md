# Repdigit

↑ **Parent:** [Integer](integer.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Repdigit)

A [repdigit](repdigit.md) is a positive integer whose base-$b$ expansion repeats one nonzero digit $d$. For $b\ge2$, $1\le d<b$ and $n\ge1$, the [finite geometric series](finite-geometric-series.md) gives $R_n=d(1+b+\cdots+b^{n-1})=d(b^n-1)/(b-1)$. For example, $5(10^n-1)/9$ has $n$ decimal digits, all equal to five.

Every [prime number](prime-number.md) not dividing $b$ divides infinitely many such [repdigits](repdigit.md). If it divides $d$, every length works. Otherwise, if it does not divide $b-1$, the [Fermat little theorem](fermat-little-theorem.md) gives divisibility for lengths that are multiples of $p-1$, and division by $b-1$ is justified by its [modular inverse](modular-multiplicative-inverse.md). If $p\mid b-1$, the sum is congruent to $dn$ modulo $p$, so lengths divisible by $p$ work instead. A prime dividing $b$ but not $d$ divides none, since $R_n\equiv d\pmod p$. This distinction prevents invalid cancellation of the geometric-sum denominator.

## ↑ Ancestors (5)

1. [Integer](integer.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4/6e/solution.md)
- [Repdigit](repdigit.md)
