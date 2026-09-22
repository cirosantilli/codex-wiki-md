<h1 id="18h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [finite field](../../../../../../finite-field.md) $\mathbb F_q$ contains a primitive tenth root exactly when $10\mid(q-1)$. Its multiplicative group is cyclic: the exponent of a finite abelian [subgroup](../../../../../../subgroup.md) of a field is attained by an element, by combining its prime-power components; since every element is a root of $X^e-1$, the [polynomial](../../../../../../polynomial-split.md) root bound forces the group order to be at most that exponent, hence equal to it. A cyclic group contains an element of order ten exactly when ten divides its order.

Over $\mathbb F_q$, the conjugates of $\xi$ are its [Frobenius automorphism](../../../../../../frobenius-automorphism.md) orbit $\xi,\xi^q,\xi^{q^2},\ldots$. The extension degree is the least $d>0$ with $q^d\equiv1\pmod{10}$. For $q=3$ this order is four, for $q=11$ it is one, and for $q=19$ it is two. Therefore

$$
\boxed{\mathbb F_3(\xi_{10})\cong\mathbb F_{81},\qquad
\mathbb F_{11}(\xi_{10})=\mathbb F_{11},\qquad
\mathbb F_{19}(\xi_{10})\cong\mathbb F_{361}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18H](../../18h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
