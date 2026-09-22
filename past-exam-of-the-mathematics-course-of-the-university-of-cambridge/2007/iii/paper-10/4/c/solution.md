<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First, all lifts of the real one-parameter projective group commute. Its scalar [commutator](../../../../../../commutator.md) $c(s,t)$ is again a continuous alternating bicharacter. For fixed nonzero $t$ and an integer $n>0$, a lift of $t$ is a phase multiple of the $n$th power of a lift of $t/n$; hence $c(t,t/n)=1$ and $c(t,mt/n)=1$ for every integer $m$. Rational multiples of $t$ are dense in $\mathbb R$, so continuity makes $c(t,s)=1$ for every $s$.

Choose a unitary $U$ representing $\rho(1)$ and the allowed [self-adjoint](../../../../../../self-adjoint-operator.md) logarithm $A\in U''$ with $U=e^{iA}$. Every lift of $\rho(t)$ commutes with $U$, hence with $A$ by the [double commutant theorem for star-algebras](../../../../../../double-commutant-theorem-for-star-algebras.md) condition. Therefore

$$
\widetilde\rho(t)=\rho(t)\,p(e^{-itA})
$$

is a continuous projective [homomorphism](../../../../../../homomorphism.md), with $\widetilde\rho(1)=1$. It is periodic of period one and descends to $\mathbb R/\mathbb Z$. Part (b) lifts it to a continuous unitary [homomorphism](../../../../../../homomorphism.md) $L$ of that [circle](../../../../../../circle.md). Each $L(t)$ is a lift of $\widetilde\rho(t)$ and commutes with $A$, since a representative has the form of an original lift times $e^{-itA}$. Thus

$$
\boxed{\widehat U_t=L(t\bmod\mathbb Z)e^{itA}}
$$

is a strongly continuous unitary [homomorphism](../../../../../../homomorphism.md) with projective class $\rho(t)$. This gives the required lift of the whole real group, not just unrelated unitary representatives at each time.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
