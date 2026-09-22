<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Now suppose $\operatorname{char}K=p>0$. The [Teichmuller lifts](../../../../../../teichmuller-representative.md) constructed in (b) are additive as well as multiplicative: if $a^q=a$ and $b^q=b$, then the characteristic-$p$ Frobenius identity gives $(a+b)^q=a^q+b^q=a+b$. Uniqueness of the lift with prescribed residue yields $[\bar a+\bar b]=[\bar a]+[\bar b]$. Their set is therefore a [finite coefficient field in positive-characteristic local fields](../../../../../../finite-coefficient-field-in-positive-characteristic-local-fields.md), and reduction identifies it with $k$.

Choose a [uniformizer](../../../../../../uniformizer.md) $\pi$. For $x\in\mathcal O_K$, let $a_0$ be the lift of its residue and write $x=a_0+\pi x_1$ with $x_1\in\mathcal O_K$. Repeat with $x_1$, then $x_2$, and so on. This gives

$$
x=\sum_{j=0}^{N}a_j\pi^j+\pi^{N+1}x_{N+1},\qquad a_j\in k\subset\mathcal O_K,quad x_{N+1}\in\mathcal O_K.
$$

The remainder tends to zero, and completeness gives $x=\sum_{j\ge0}a_j\pi^j$. The expansion is unique: in a nonzero difference of two series the first different coefficient is a nonzero element of the coefficient field, hence a unit, and so gives exactly the valuation of that difference.

Consequently substitution $t\mapsto\pi$ defines a bijection $k[[t]]\to\mathcal O_K$. It is a ring homomorphism because the coefficient lift is a field homomorphism, polynomial operations agree before passage to limits, and multiplication is continuous. Every element of $K$ becomes integral after multiplication by a sufficiently large power of $\pi$. Allowing finitely many negative powers therefore extends substitution to the field isomorphism

$$
\boxed{k((t))\xrightarrow{\sim}K,\qquad\sum_{j\ge m}a_jt^j\longmapsto\sum_{j\ge m}a_j\pi^j.}
$$

It preserves the normalized [discrete valuation](../../../../../../discrete-valuation.md), since the first nonzero coefficient determines the valuation on each side. The results used are the structural facts stated in (a), its proved [Hensel lemma](../../../../../../hensel-s-lemma.md), the proved multiplicative lifting in (b), and the characteristic-$p$ identity $(a+b)^q=a^q+b^q$. No classification theorem for local fields is needed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
