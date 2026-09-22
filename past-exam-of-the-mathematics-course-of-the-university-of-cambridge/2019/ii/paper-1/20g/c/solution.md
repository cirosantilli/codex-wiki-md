<h1 id="20g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\varepsilon=1+\sqrt2$ and $P=(3+\sqrt2)$. The generator of this [principal ideal](../../../../../../principal-ideal.md) has norm

$$
N_{K/\mathbb Q}(3+\sqrt2)=9-2=7.
$$

Reduction modulo $P$ gives $\sqrt2\equiv-3\equiv4\pmod7$. The map below is surjective and has $P$ in its kernel; both the kernel and $P$ have index seven, the latter by the [ideal norm](../../../../../../ideal-norm.md), so they are equal. Hence it induces an isomorphism of [residue fields](../../../../../../residue-field.md)

$$
\mathcal O_K/P\cong\mathbb F_7,
\qquad
a+b\sqrt2\longmapsto a+4b\pmod7.
$$

In particular,

$$
\varepsilon\equiv5\pmod P.
$$

In the [finite field](../../../../../../finite-field.md) $\mathbb F_7$, the element $5$ has multiplicative order six, since

$$
5^2\equiv4,
\qquad
5^3\equiv-1,
\qquad
5^6\equiv1\pmod7.
$$

By part (b), every unit is $(-1)^\delta\varepsilon^n$ for $\delta\in\{0,1\}$ and $n\in\mathbb Z$. Since $-1\equiv5^3$, its residue is $5^{n+3\delta}$, which equals one exactly when

$$
n+3\delta\equiv0\pmod6.
$$

The resulting units are $\varepsilon^{6k}$ and $-\varepsilon^{6k+3}$, and these are precisely the even and odd powers of $-\varepsilon^3$. Therefore

$$
\boxed{G=\langle-\varepsilon^3\rangle
=\left\langle-(1+\sqrt2)^3\right\rangle
=\langle-7-5\sqrt2\rangle},
$$

which is the group of [units congruent to one modulo 3 plus square root two](../../../../../../units-congruent-to-one-modulo-3-plus-square-root-two.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [20G](../../20g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
