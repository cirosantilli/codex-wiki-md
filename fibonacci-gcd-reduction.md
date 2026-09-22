# Fibonacci gcd reduction

↑ **Parent:** [Fibonacci addition formula](fibonacci-addition-formula.md)

Consecutive [Fibonacci numbers](fibonacci-number.md) are [coprime](coprime-integers.md) by the [Euclidean algorithm](euclidean-algorithm.md). The [Fibonacci addition formula](fibonacci-addition-formula.md) writes $F_m=F_{m-n}F_{n+1}+F_{m-n-1}F_n$ for $m>n$. Taking the [greatest common divisor](greatest-common-divisor.md) with $F_n$ removes the last summand, and multiplication by the [coprime](coprime-integers.md) factor $F_{n+1}$ leaves that gcd unchanged. The case $m=n$ uses $F_0=0$. Applying the [Euclidean algorithm](euclidean-algorithm.md) to the indices yields the strong-divisibility identity $\gcd(F_m,F_n)=F_{\gcd(m,n)}$ for nonnegative indices, with the usual zero conventions.

## ↑ Ancestors (8)

1. [Fibonacci addition formula](fibonacci-addition-formula.md)
2. [Fibonacci number](fibonacci-number.md)
3. [Sequence and series](sequence-and-series.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-4/7c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-4/8e/solution.md)
