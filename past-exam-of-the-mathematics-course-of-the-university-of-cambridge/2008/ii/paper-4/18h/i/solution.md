<h1 id="18h/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The automorphisms satisfy $\sigma^n=\tau^2=1$ and $\tau\sigma\tau=\sigma^{-1}$. The $n$ rotations $z\mapsto\zeta_n^jz$ and $n$ inversion maps $z\mapsto\zeta_n^j/z$ are all distinct, so the [dihedral group](../../../../../../dihedral-group.md) $G$ has order $2n$, including the case $n=1$ when it has order two. The invariant

$$
\boxed{w=z^n+z^{-n}}
$$

is fixed by both generators.

Use two standard field-theoretic results: the fixed-field theorem for a finite group of automorphisms gives $[L:L^G]=|G|$ and makes $L/L^G$ Galois with group $G$; and a nonconstant rational function $P(z)/Q(z)$ in lowest terms satisfies $[\mathbb C(z):\mathbb C(P/Q)]=\max(\deg P,\deg Q)$. Here $w=(z^{2n}+1)/z^n$ has coprime numerator and denominator and degree $2n$. Thus $[L:\mathbb C(w)]=[L:L^G]=2n$. Since $\mathbb C(w)\subseteq L^G$, the tower law proves the [dihedral fixed field in one rational variable](../../../../../../dihedral-fixed-field-in-one-rational-variable.md):

$$
\boxed{L^G=\mathbb C(z^n+z^{-n}).}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [18H](../../18h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
