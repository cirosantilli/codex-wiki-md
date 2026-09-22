# Miller-Rabin primality test

↑ **Parent:** [Primality testing](primality-testing.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Miller–Rabin_primality_test)

For an odd candidate $n>3$, write $n-1=2^s d$ with $d$ odd. A base $a$ passes when $a^d\equiv1\pmod n$ or $a^{2^jd}\equiv-1\pmod n$ for some $0\le j<s$; a nontrivial common divisor of $a,n$ or failure of these conditions proves compositeness. A prime passes every base, while an odd composite passes at most one quarter of possible bases. Independent rounds give a false probable-prime probability at most $4^{-r}$. A passing composite is a [strong pseudoprime](strong-pseudoprime.md), stronger than a [Fermat pseudoprime](fermat-pseudoprime.md).

## ↑ Ancestors (5)

1. [Primality testing](primality-testing.md)
2. [Computational complexity theory](computational-complexity-theory.md)
3. [Theoretical computer science](theoretical-computer-science.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3/11g/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3/11g/solution.md)
