<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Reduce $P$ to $\overline P\in\widetilde E(\mathbb F_p)$. Because $p\nmid n$, the [multiplication-by-n morphism](../../../../../../multiplication-by-n-morphism.md) on the reduced [elliptic curve](../../../../../../elliptic-curve.md) is a separable, surjective morphism of degree $n^2$. Choose a point $\overline Q\in\widetilde E(\overline{\mathbb F}_p)$ with $n\overline Q=\overline P$. Its coordinates lie in some finite field $\mathbb F_{p^d}$.

Let $L/\mathbb Q_p$ be the finite [unramified extension](../../../../../../unramified-extension.md) with residue field $\mathbb F_{p^d}$. The curve retains [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md) over $L$. Its smooth integral model and the [Hensel lemma](../../../../../../hensel-s-lemma.md) give [surjectivity of good reduction over a local field](../../../../../../surjectivity-of-good-reduction-over-a-local-field.md), so lift $\overline Q$ to some $Q_0\in E(L)$. This lift need not satisfy $nQ_0=P$ exactly, but its error

$$
R=P-nQ_0
$$

has zero reduction and belongs to $E_1(L)$, the [kernel of reduction of an elliptic curve](../../../../../../kernel-of-reduction-of-an-elliptic-curve.md).

The parameter $t=-x/y$ at infinity identifies $E_1(L)$ with the maximal ideal $\mathfrak m_L$ equipped with the [formal group of an elliptic curve](../../../../../../formal-group-of-an-elliptic-curve.md). The integral power series for $[n]$ and its inverse from part (i) remain integral over $\mathcal O_L$. They converge on $\mathfrak m_L$: terms of degree $k$ tend to zero in valuation because their coefficients are integral and the argument has positive valuation. Hence multiplication by $n$ is bijective on $E_1(L)$. Choose its unique solution $T\in E_1(L)$ to $nT=R$, and put $Q=Q_0+T$. Then

$$
\boxed{Q\in E(L),\qquad nQ=nQ_0+R=P,\qquad L/\mathbb Q_p\text{ finite unramified}.}
$$

The residue-field extension supplies a division point modulo $p$, and the formal-group inverse corrects the error without introducing ramification. This is the local construction underlying the [uniform unramified division field over a local field](../../../../../../uniform-unramified-division-field-over-a-local-field.md) and [unramified division torsors at good primes](../../../../../../unramified-division-torsors-at-good-primes.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
