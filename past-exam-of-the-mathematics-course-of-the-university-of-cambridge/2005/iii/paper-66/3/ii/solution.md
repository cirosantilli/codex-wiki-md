<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

There are no numerical [continuity](../../../../../../continuous-function.md) bounds determined by $w$ and $a$ alone: the [subdivision mask](../../../../../../subdivision-mask.md) coefficients matter. First check constant reproduction, $\sum_jM_{\epsilon-aj}=1$ for every residue $\epsilon$, and convergence. For the usual stationary [scalar](../../../../../../scalar.md) scheme, two useful calculations are a uniform contraction test and a spectral obstruction test. Higher smoothness is tested with derived difference [subdivision masks](../../../../../../subdivision-mask.md).

Write $M(z)=\sum_jM_jz^j$ and $s_a(z)=1+z+\cdots+z^{a-1}$. Using backward differences $\Delta P_i=P_i-P_{i-1}$, the generating-function identity

$$
(1-z)M(z)=\frac{M(z)}{s_a(z)}(1-z^a)
$$

proves the [subdivision difference scheme](../../../../../../subdivision-difference-scheme.md) relation $\Delta S_M=S_{M/s_a}\Delta$. Iterating gives $\Delta^rS_M=S_{M/s_a^r}\Delta^r$. To test a candidate $C^r$ limit, suppose the requisite sum rules hold, so $M/s_a^{r+1}$ is a finite [Laurent polynomial](../../../../../../laurent-polynomial.md). The scaled [derivative](../../../../../../derivative.md) controls $q_i^\ell=a^{r\ell}\Delta^rP_i^\ell$ are refined by the [subdivision mask](../../../../../../subdivision-mask.md)

$$
D_r(z)=a^r\frac{M(z)}{s_a(z)^r},
$$

whose residue sums are one. Their first differences are refined by

$$
B_r(z)=a^r\frac{M(z)}{s_a(z)^{r+1}}.
$$

The powers of $a$ are essential because each refinement shrinks parameter intervals by $a$.

**A lower [continuity](../../../../../../continuous-function.md) bound comes from proving uniform contraction.** The infinity norm of one difference-refinement step is bounded by

$$
q=\max_{0\le\epsilon<a}\sum_j|(B_r)_{\epsilon-aj}|.
$$

If $q<1$, adjacent [derivative](../../../../../../derivative.md) controls contract geometrically at every location. More generally, form the $p$-step [subdivision mask](../../../../../../subdivision-mask.md)

$$
B_r^{[p]}(z)=\prod_{\nu=0}^{p-1}B_r(z^{a^\nu})
$$

and test $\max_{\epsilon\bmod a^p}\sum_j|(B_r^{[p]})_{\epsilon-a^pj}|<1$. This proves convergence of the constant-preserving [derivative](../../../../../../derivative.md) scheme to a continuous limit. One justification is to compare consecutive piecewise-linear interpolants: their difference is bounded by a constant times the maximum adjacent-control difference, and the geometrically decreasing bound is summable. To identify the limit as $P^{(r)}$, use fixed-degree [Cardinal B-spline](../../../../../../cardinal-b-spline.md) interpolants of the original refined controls. Their $r$th [derivatives](../../../../../../derivative.md) are sums of the scaled [finite differences](../../../../../../finite-difference-split.md); convergence of both functions and [derivatives](../../../../../../derivative.md) gives $P\in C^r$. Testing successive $r$ supplies a guaranteed [lower bound](../../../../../../lower-bound-in-a-partially-ordered-set.md).

**An upper [continuity](../../../../../../continuous-function.md) bound comes from an observable noncontracting shape mode.** Build finite local [subdivision matrices](../../../../../../subdivision-matrix.md) for $B_r$ on a refinement-invariant control neighborhood. For a digit $\epsilon$ their entries are $(A_\epsilon)_{ij}=(B_r)_{\epsilon+i-aj}$, since the new index is $ak+\epsilon+i$. Restrict to the realizable difference space and discard modes that do not affect the limit. A word $\epsilon_1,\ldots,\epsilon_p$ corresponds to a nested parameter location. If its product has an observable [eigenvalue](../../../../../../eigenvalue.md) $\lambda$ with $|\lambda|>1$, repetition of this word makes some scaled [derivative](../../../../../../derivative.md) differences grow rather than tend to zero. For a stable limit representation, $C^r$ regularity would force these differences to vanish; hence general-position data cannot have $C^r$ [continuity](../../../../../../continuous-function.md). A modulus-one mode requires examination of whether it actually persists, rather than an automatic rounding rule.

The two calculations can be organized through the [joint spectral radius](../../../../../../joint-spectral-radius.md) $\widehat\rho$ of these restricted [matrices](../../../../../../matrix.md):

$$
\boxed{\max_{|\epsilon|=p}\rho(A_{\epsilon_p}\cdots A_{\epsilon_1})^{1/p}\le\widehat\rho\le\max_{|\epsilon|=p}\|A_{\epsilon_p}\cdots A_{\epsilon_1}\|^{1/p}.}
$$

These [norm and spectral bounds for subdivision regularity](../../../../../../norm-and-spectral-bounds-for-subdivision-regularity.md) make the test computable from the [subdivision mask](../../../../../../subdivision-mask.md). The right bound certifies all-word contraction when it is less than one; the left bound detects a repeated-word obstruction when it exceeds one. Longer products improve the tests. A single [matrix](../../../../../../matrix.md)'s spectrum is not a substitute for controlling arbitrary products. The product estimates also appear in [Charina's analysis of subdivision regularity](https://arxiv.org/pdf/1202.2765); the strict contraction and observable-mode arguments above explain their respective roles.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
