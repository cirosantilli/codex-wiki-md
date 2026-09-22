<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $h$ be the standard Cartan element of the [sl2 Lie algebra](../../../../../../sl2-lie-algebra.md), with $[h,e]=2e$ and $[h,f]=-2f$. For a finite-dimensional representation, its [formal character](../../../../../../formal-character-of-a-weight-module.md) records its [weight multiplicities](../../../../../../weight-multiplicity.md):

$$
\boxed{\chi_V(q)=\sum_{j\in\mathbb Z}(\dim V_j)q^j,\qquad
V_j=\{v:hv=jv\}.}
$$

The [classification of finite-dimensional sl2 representations](../../../../../../classification-of-finite-dimensional-sl2-representations.md) and the [Weyl complete reducibility theorem](../../../../../../weyl-complete-reducibility-theorem.md) give $V=\bigoplus_{m\ge0}a_mL_m$, with finitely many nonzero $a_m$. Each $L_m$ has [weights](../../../../../../weight-representation-theory.md) $m,m-2,\ldots,-m$, each of multiplicity one. Therefore

$$
\chi_V(q)=\sum_{m\ge0}a_m(q^m+q^{m-2}+\cdots+q^{-m}),
\qquad c_j=\sum_{\substack{m\ge |j|\\m\equiv j\ (2)}}a_m.
$$

In particular $c_j=c_{-j}$, and for $j\ge0$ one has $c_j-c_{j+2}=a_j\ge0$. This proves [parity unimodality of an sl2 character](../../../../../../parity-unimodality-of-an-sl2-character.md): **within each parity, the coefficients increase towards zero and decrease away from zero**. For a representation whose [weights](../../../../../../weight-representation-theory.md) have a single parity, deleting the intervening zero coefficients gives a symmetric unimodal sequence.

The parity convention is necessary for the printed assertion. If unimodality means the full coefficient sequence at every consecutive integer exponent, it is false: the standard two-dimensional representation has character $q+q^{-1}$, whose coefficients at exponents $-1,0,1$ are $1,0,1$. The statement established above is unimodality on cosets of the [root lattice](../../../../../../root-lattice.md) for $\mathfrak{sl}_2$, and is the version needed in part ii. Infinite-dimensional representations need not even have Laurent-polynomial characters.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
