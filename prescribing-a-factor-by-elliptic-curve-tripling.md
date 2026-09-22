# Prescribing a factor by elliptic-curve tripling

↑ **Parent:** [Elliptic curve method](elliptic-curve-method.md)

Let $N=pq$ with [primes](prime-number-split.md) $p\equiv1\pmod{12}$ and $q\equiv5\pmod{12}$. [quadratic reciprocity](quadratic-reciprocity.md) makes three a square modulo $p$; choose $r^2=3$ and impose $a=-3+2r\pmod p$, $a=1\pmod q$ by the [Chinese remainder theorem](chinese-remainder-theorem.md). The curve has good reduction at both [primes](prime-number-split.md). Indeed its discriminant is $-16a^2(4a+27)$; the first condition could make a factor vanish only at $p=3$ or 11, while the second gives $a(4a+27)=31$ and the given residue class excludes $q=31$.

Doubling $P$ gives $x(2P)-1=(a^2+6a-3)/4$. This vanishes modulo $p$ and equals one modulo $q$. Modulo $p$ one also has $y(2P)=-1$, so $2P=-P$ and $3P$ is the identity. Modulo $q$ the addition is finite. Thus computing $3P$ modulo $N$ encounters a denominator whose [greatest common divisor](greatest-common-divisor.md) with $N$ is exactly $p$, revealing the factor. The numerator difference is minus two modulo $p$, so the failed inverse cannot be cancelled. This is a construction of successful [elliptic curve method](elliptic-curve-method.md) data from prescribed local group behavior.

## ↑ Ancestors (10)

1. [Elliptic curve method](elliptic-curve-method.md)
2. [Elliptic curve](elliptic-curve.md)
3. [Genus one curve](genus-one-curve.md)
4. [Geometric genus](geometric-genus.md)
5. [Normalization of an algebraic curve](normalization-of-an-algebraic-curve-split.md)
6. [Algebraic geometry](algebraic-geometry-split.md)
7. [Geometry and topology](geometry-and-topology-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford/2008/b/8/c/solution.md)
