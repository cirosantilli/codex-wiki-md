<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Every [automorphism](../../../../automorphism.md) fixes zero and one, and preserves sums, products, negatives and multiplicative inverses of nonzero elements. Consequently elements fixed by every member of $G$ are closed under these operations and form a [field](../../../../field.md). [Artin fixed-field theorem](../../../../artin-fixed-field-theorem.md) gives $\boxed{[L:L^G]=|G|}$ for a finite [automorphism](../../../../automorphism.md) [group](../../../../group-split.md).

Here $\mathbb Q(t)$ is the fraction [field](../../../../field.md) of $\mathbb Q[t]$, with $t$ transcendental; its elements are fractions of rational-coefficient [polynomials](../../../../polynomial-split.md), with nonzero denominator and the usual equality by cross-multiplication. Substitution of $1-t$ or $1/t$ defines an [automorphism](../../../../automorphism.md), each its own inverse. With $\sigma\tau$ meaning first apply $\tau$ to a [field](../../../../field.md) element and then $\sigma$, its image on $t$ is $1/(1-t)$. Iterating gives $(t-1)/t$ and then $t$, so its order is three. The relations reduce every word to at most six possibilities, and the six resulting images are

$$
t,\quad1-t,\quad1/t,\quad1/(1-t),\quad(t-1)/t,\quad t/(t-1).
$$

They are distinct [rational functions](../../../../rational-function.md), so the [group](../../../../group-split.md) has six elements. Its faithful [permutation](../../../../permutation.md) action on $\{0,1,\infty\}$ identifies it with $\boxed{S_3}$.

For the first [fixed field](../../../../fixed-field.md) put $u=t(1-t)$. It is fixed by $\sigma$, and $t$ satisfies $X^2-X+u=0$ over $\mathbb Q(u)$. The degree is exactly two because the nontrivial [automorphism](../../../../automorphism.md) $\sigma$ fixes that [field](../../../../field.md). The fixed-[field](../../../../field.md) degree is also two, so

$$
\boxed{\mathbb Q(t)^{\langle\sigma\rangle}=\mathbb Q(t(1-t)).}
$$

For the inversion put $v=t+1/t$. It is fixed and $t$ satisfies $X^2-vX+1=0$. The same degree argument gives

$$
\boxed{\mathbb Q(t)^{\langle\tau\rangle}=\mathbb Q(t+1/t).}
$$

The source requests [polynomial](../../../../polynomial-split.md) generators in both cases. The second requirement is impossible. If a nonconstant [polynomial](../../../../polynomial-split.md) $p(t)=a_dt^d+\cdots+a_0$ were fixed by inversion, $p(t)=p(1/t)$ would equate a [Laurent polynomial](../../../../laurent-polynomial.md) with highest exponent $d>0$ to one with no positive exponent, a contradiction. Thus the only [polynomial](../../../../polynomial-split.md) invariants of inversion are constants, which cannot generate its nonconstant [fixed field](../../../../fixed-field.md). The [fixed field of inversion in a rational function field](../../../../fixed-field-of-inversion-in-a-rational-function-field.md) therefore has the second displayed rational-function generator.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the number theory course of the University of Oxford](../../../split.md)
5. [Number theory course of the University of Oxford](../../../../number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
