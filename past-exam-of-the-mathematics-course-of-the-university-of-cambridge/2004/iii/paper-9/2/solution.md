<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the extended-value convention for a [normal family](../../../../../normal-family.md), which is essential here: every sequence in the holomorphic family has a subsequence converging uniformly on [compact](../../../../../compact-space.md) subsets either to a finite [holomorphic function](../../../../../holomorphic-function.md) or to infinity. Convergence to infinity means $\inf_K|f_n|\to\infty$ for every [compact](../../../../../compact-space.md) $K\subset D$. Equivalently one uses local [uniform convergence](../../../../../uniform-convergence.md) in the [chordal metric](../../../../../chordal-metric.md). For [holomorphic functions](../../../../../holomorphic-function.md) a nonconstant meromorphic limit cannot acquire a [pole](../../../../../pole.md): near a supposed [pole](../../../../../pole.md), the reciprocals of sufficiently large-index functions are holomorphic and nowhere zero, and converge to a [holomorphic function](../../../../../holomorphic-function.md) with a zero. [Hurwitz's theorem](../../../../../hurwitz-s-theorem.md) would force that reciprocal limit to vanish identically, giving the constant infinite limit instead.

Restriction proves that global normality implies normality near each point. For the converse, choose a countable cover by [connected](../../../../../connected-space.md) discs $U_j$ on which the family is normal, with smaller discs covering $D$ and having [compact](../../../../../compact-space.md) closure inside the corresponding $U_j$. Such a cover exists from the countable rational-disc basis and local normality. Starting with any sequence, extract a subsequence converging on $U_1$, then a further subsequence converging on $U_2$, and so on. The diagonal sequence converges on each $U_j$. On an overlap the limits agree; a finite holomorphic limit and infinity cannot both occur there. The overlap graph of this cover is [connected](../../../../../connected-space.md), since otherwise its components would partition the [connected](../../../../../connected-space.md) domain into disjoint open subsets. Therefore all local limits are of the same type and patch to one [holomorphic function](../../../../../holomorphic-function.md) or to infinity throughout $D$. Every [compact set](../../../../../compact-space.md) has a finite cover by the smaller discs, so convergence on their [compact](../../../../../compact-space.md) closures gives [uniform convergence](../../../../../uniform-convergence.md) on that [compact set](../../../../../compact-space.md). This proves that [normality is a local property](../../../../../normality-is-a-local-property.md).

For the counterexample take the [unit disc](../../../../../unit-disc.md) and the family $f_n(z)=n(1+z^2/2)$. Since $|1+z^2/2|\ge1-|z|^2/2>1/2$, $f_n$ tends uniformly to infinity. Any sequence from this family either has a constant subsequence or has indices tending to infinity, so the family is normal. Its [derivatives](../../../../../derivative.md) are $nz$. No subsequence of these [derivatives](../../../../../derivative.md) can have a finite locally uniform limit, because their values at any fixed nonzero point grow without bound; nor can they tend locally uniformly to infinity, since every [derivative](../../../../../derivative.md) vanishes at zero. Thus **a holomorphic [normal family](../../../../../normal-family.md) need not have a normal [derivative](../../../../../derivative.md) family**.

Now impose the point bound at $z_0$. For any sequence of [derivatives](../../../../../derivative.md) choose corresponding functions from the original family. Normality supplies a locally uniformly convergent subsequence, and the point bound excludes the infinite limit. Let its finite holomorphic limit be $f$. The [Cauchy integral formula](../../../../../cauchy-integral-formula.md) gives convergence of [derivatives](../../../../../derivative.md) uniformly on [compact](../../../../../compact-space.md) subsets. Explicitly, for [compact](../../../../../compact-space.md) $K\subset D$ choose $\rho>0$ so its closed $\rho$-neighborhood lies in a [compact](../../../../../compact-space.md) $L\subset D$; then

$$
\sup_{z\in K}|f_n'(z)-f'(z)|\le\rho^{-1}\sup_{\zeta\in L}|f_n(\zeta)-f(\zeta)|\longrightarrow0.
$$

Every sequence of [derivatives](../../../../../derivative.md) therefore has a locally uniform subsequential limit. This [pointwise anchoring of a holomorphic normal family](../../../../../pointwise-anchoring-of-a-holomorphic-normal-family.md) proves **the [derivative](../../../../../derivative.md) family is normal under the stated bound**.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
