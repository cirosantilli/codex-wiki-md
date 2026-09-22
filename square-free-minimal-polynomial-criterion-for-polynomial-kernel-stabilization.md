# Square-free minimal polynomial criterion for polynomial kernel stabilization

↑ **Parent:** [Minimal polynomial](minimal-polynomial.md)

For a [linear operator](linear-operator.md) on a finite-dimensional [vector space](vector-space-split.md) over a [field](field.md) $K$, all polynomial kernels stabilize at their first power exactly when its [minimal polynomial](minimal-polynomial.md) $m$ has no repeated [irreducible polynomial](irreducible-polynomial.md) factor in $K[X]$. This formulation does not require those factors to be linear.

To prove it, the [Bézout's identity for polynomials](bezout-s-identity-for-polynomials.md) gives $\ker q(T)=\ker\gcd(q,m)(T)$: a greatest common divisor is a combination of $q$ and $m$, while $q$ is its multiple. If $m$ is square-free, $\gcd(p^n,m)=\gcd(p,m)$, proving the displayed equality. Conversely, if an irreducible factor $f$ occurs to exponent $e\ge2$, its [primary decomposition theorem](primary-decomposition-theorem-for-linear-maps.md) summand has [minimal polynomial](minimal-polynomial.md) $f^e$. On this summand $f(T)$ is nonzero, while $f(T)^e=0$. Thus the kernels of those two powers differ. An [eigenbasis](eigenbasis.md) follows from this criterion precisely when the distinct factors of $m$ are also linear over $K$; a real rotation through a right angle has square-free $m=X^2+1$ but no real [eigenvalues](eigenvalue.md).

## ↑ Ancestors (7)

1. [Minimal polynomial](minimal-polynomial.md)
2. [Operator theory](linear-operator-theory-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-2-course-of-the-university-of-oxford/2004/2/ii/solution.md)
