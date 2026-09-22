<h1 id="23f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a measurable set $E\subseteq U$, define

$$
\nu(E)=\Lambda(\mathbf1_E),
$$

where $\mathbf1_E$ is its [indicator function](../../../../../../indicator-function.md). This is finite because $U$ has [finite measure](../../../../../../finite-measure.md) and hence $\mathbf1_E\in L^p(U)$. If the sets $E_k$ are pairwise disjoint and $E=\bigcup_{k\geq1}E_k$, then

$$
\left\|\mathbf1_E-
\sum_{k=1}^N\mathbf1_{E_k}\right\|_p^p
=|E\setminus\bigcup_{k=1}^NE_k|\longrightarrow0.
$$

The continuity of the [positive linear functional](../../../../../../positive-linear-functional.md) $\Lambda$ therefore gives

$$
\nu(E)=\sum_{k=1}^{\infty}\nu(E_k),
$$

so $\nu$ is a [measure](../../../../../../measure.md) by [countable additivity](../../../../../../countable-additivity.md). Moreover, a set of zero [Lebesgue measure](../../../../../../lebesgue-measure.md) has zero indicator in $L^p$, so $\nu$ is [absolutely continuous](../../../../../../absolute-continuity-of-measures.md) with respect to Lebesgue measure.

The [Radon-Nikodym theorem](../../../../../../radon-nikodym-theorem.md) now supplies a measurable function $\omega\geq0$ such that

$$
\nu(E)=\int_E\omega.
$$

Consequently, first for nonnegative simple functions and then, by [approximation by nonnegative simple functions](../../../../../../approximation-by-nonnegative-simple-functions.md), for every nonnegative $f\in L^p(U)$,

$$
\int_U f\omega=\Lambda(f)
\leq\|\Lambda\|\,\|f\|_p.
$$

Applying the stated characterization of the [Lp norm](../../../../../../lp-norm.md) to $\omega$ shows that $\omega\in L^q(U)$ and $\|\omega\|_q\leq\|\Lambda\|$. The [Holder inequality](../../../../../../holder-inequality.md) makes $f\mapsto\int_Uf\omega$ continuous on $L^p(U)$, while bounded simple functions form a [dense subset](../../../../../../dense-set.md); hence

$$
\boxed{\Lambda(f)=\int_U f\omega\quad(f\in L^p(U)).}
$$

This is the [positive functional representation on Lp](../../../../../../positive-functional-representation-on-lp.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [23F](../../23f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
