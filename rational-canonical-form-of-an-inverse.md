# Rational canonical form of an inverse

↑ **Parent:** [Rational canonical form](rational-canonical-form.md)

Let an [invertible matrix](invertible-matrix.md) $T$ have monic [invariant factors of a linear operator](invariant-factors-of-a-linear-operator.md) $f_j$ of degrees $d_j$. Their constant coefficients are nonzero, since their product is the [characteristic polynomial](characteristic-polynomial.md) and $\det T\ne0$. On a cyclic block, $f(T)=0$ implies $T^{-d}f(T)=0$, so $f^\vee(T^{-1})=0$, where $f^\vee(t)=t^df(1/t)/f(0)$ is monic of degree $d$. The vector $v$ remains cyclic for $T^{-1}$: multiplying $v,T^{-1}v,\ldots,T^{-(d-1)}v$ by the invertible map $T^{d-1}$ gives the reversed original cyclic basis. Thus this polynomial is the [minimal polynomial](minimal-polynomial.md) of the inverse block.

Normalized reciprocation preserves divisibility because $(fg)^\vee=f^\vee g^\vee$ when both constant coefficients are nonzero. Consequently the [rational canonical form](rational-canonical-form.md) of $T^{-1}$ is the direct sum of the [companion matrices](companion-matrix.md) $C(f_j^\vee)$. The normalization by $f_j(0)$ is essential to make each reciprocal polynomial monic.

## ↑ Ancestors (7)

1. [Rational canonical form](rational-canonical-form.md)
2. [Operator theory](linear-operator-theory-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-rings-and-modules-course-of-the-university-of-oxford/2017/3/c/solution.md)
