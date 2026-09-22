<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The ambient [group ring of a weight lattice](../../../../../../group-ring-of-a-weight-lattice.md) is

$$
\mathbb Z[\Lambda_W]=\left\{\sum_{\lambda\in\Lambda_W}a_\lambda e(\lambda):
a_\lambda\in\mathbb Z,\text{ with finite support}\right\},
\qquad e(\lambda)e(\mu)=e(\lambda+\mu).
$$

Addition is coefficientwise, and multiplication uses addition in the [weight lattice](../../../../../../weight-lattice.md). For a finite-dimensional [Lie algebra representation](../../../../../../lie-algebra-representation.md) $V=\bigoplus_\lambda V_\lambda$, its [formal character](../../../../../../formal-character-of-a-weight-module.md) is

$$
\boxed{\operatorname{char}V=\sum_\lambda(\dim V_\lambda)e(\lambda).}
$$

The [formal character](../../../../../../formal-character-of-a-weight-module.md) records the [dimensions](../../../../../../dimension-vector-space.md) of all [weight spaces](../../../../../../weight-space.md). The ambient lattice ring should be distinguished from the [representation ring of a semisimple Lie algebra](../../../../../../representation-ring-of-a-semisimple-lie-algebra.md), which identifies with its Weyl-invariant subring.

For the $\mathfrak{sl}_3$ module $\Gamma_{1,2}$, $L_1+L_2+L_3=0$ and the [highest weight](../../../../../../highest-weight-of-a-representation.md) is $L_1-2L_3=\omega_1+2\omega_2$. The decomposition $V\otimes\operatorname{Sym}^2V^*=\Gamma_{1,2}\oplus V^*$ gives

$$
\operatorname{char}\Gamma_{1,2}
=\left(\sum_i e(L_i)\right)\left(\sum_{j\leq k}e(-L_j-L_k)\right)-\sum_i e(-L_i).
$$

Collecting equal [weights](../../../../../../weight-representation-theory.md) yields

$$
\boxed{\operatorname{char}\Gamma_{1,2}
=\sum_{i\ne j}e(L_i-2L_j)+\sum_{i=1}^3e(2L_i)+2\sum_{i=1}^3e(-L_i).}
$$

The six first [weights](../../../../../../weight-representation-theory.md) and three second [weights](../../../../../../weight-representation-theory.md) have multiplicity one; each of the three [weights](../../../../../../weight-representation-theory.md) $-L_i$ has multiplicity two. Their total is $6+3+6=15$, as required.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
