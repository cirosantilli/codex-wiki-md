<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If $\phi=T'\psi$ and $v\in\ker T$, then $\phi(v)=\psi(Tv)=0$. Thus $\operatorname{im}T'\subseteq(\ker T)^\circ$, using the [annihilator of a vector subspace](../../../../../annihilator-of-a-vector-subspace.md).

Conversely, let $\phi$ vanish on the [kernel of a linear map](../../../../../kernel-of-a-linear-map-split.md) $\ker T$. Define a [linear functional](../../../../../linear-functional.md) on $\operatorname{im}T$ by $\psi_0(Tv)=\phi(v)$. This is well-defined: $Tv=Tw$ implies $v-w\in\ker T$, so $\phi(v)=\phi(w)$. Extend $\psi_0$ to a [linear functional](../../../../../linear-functional.md) $\psi$ on $W$, using the extension argument from part (i). Then $T'\psi=\phi$, proving

$$
\boxed{\operatorname{im}T'=(\ker T)^\circ.}
$$

The dimension formula from part (i) and the [rank-nullity theorem](../../../../../rank-nullity-theorem.md) now give

$$
\operatorname{rank}T'=\dim(\ker T)^\circ
=\dim V-\dim\ker T=\operatorname{rank}T.
$$

To deduce the [eigenvalue](../../../../../eigenvalue.md) statement, apply this equality of [rank of a linear map](../../../../../rank-of-a-linear-map.md) to $T-\lambda I$. Its [dual map](../../../../../transpose-of-a-linear-map.md) is $T'-\lambda I$, so their [kernel of a linear map](../../../../../kernel-of-a-linear-map-split.md) dimensions agree. Thus the same $\lambda$ are [eigenvalues](../../../../../eigenvalue.md), with the same [geometric multiplicities](../../../../../geometric-multiplicity.md).

For [algebraic multiplicities](../../../../../algebraic-multiplicity.md) as well, part (a)(iii) gives

$$
\bigl((T-\lambda I)^r\bigr)'=(T'-\lambda I)^r,
$$

so equality of [rank](../../../../../rank-of-a-linear-map.md) applies to every power. Hence

$$
\dim\ker(T-\lambda I)^r=\dim\ker(T'-\lambda I)^r.
$$

After extending to a [field](../../../../../field.md) where the [characteristic polynomials](../../../../../characteristic-polynomial.md) split, take $r\geq\dim V$. These [kernel of a linear map](../../../../../kernel-of-a-linear-map-split.md) spaces are the [generalized eigenspaces](../../../../../generalized-eigenspace.md); the [primary decomposition theorem for linear maps](../../../../../primary-decomposition-theorem-for-linear-maps.md) identifies their dimensions with the [algebraic multiplicities](../../../../../algebraic-multiplicity.md). The same proof works over the original [field](../../../../../field.md) for every [eigenvalue](../../../../../eigenvalue.md) in it. We obtain

$$
\boxed{\text{$T$ and $T'$ have the same nonzero eigenvalues,
with both kinds of multiplicity equal.}}
$$

In fact the argument also includes the zero [eigenvalue](../../../../../eigenvalue.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the linear algebra course of the University of Oxford](../../../../split.md)
6. [Linear algebra course of the University of Oxford](../../../../../linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
