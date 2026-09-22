<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use four-dimensional Minkowski signature $(+---)$, $\sigma^\mu=(I,\sigma^i)$ and $\bar Q_{\dot\alpha}=(Q_\alpha)^\dagger$. The odd [supercharges](../../../../../../supersymmetry-generator.md) transform as a [Weyl spinor](../../../../../../weyl-spinor.md) and its conjugate. In the ordinary particle [Super-Poincaré algebra](../../../../../../super-poincare-algebra.md), [Lorentz covariance](../../../../../../lorentz-covariance.md) makes the mixed anticommutator a vector, since $(1/2,0)\otimes(0,1/2)=(1/2,1/2)$. The even vector generator is the translation generator $P_\mu$, so the anticommutator is a real normalization constant times $\sigma^\mu P_\mu$. Unitarity makes that constant positive, and rescaling the charges sets it to two.

The same-chirality anticommutator is symmetric in its two spinor indices. A Lorentz-scalar term would require $\epsilon_{\alpha\beta}$ and hence an antisymmetric internal charge label, unavailable for $\mathcal N=1$. A term in the Lorentz generators would violate the translation Jacobi identity. Excluding additional tensorial brane charges, as in the ordinary particle algebra, the same-chirality anticommutators therefore vanish. Lorentz covariance could initially allow $[P_\mu,Q_\alpha]=a\sigma_{\mu\alpha\dot\gamma}\bar Q^{\dot\gamma}$. The [graded Jacobi identity](../../../../../../graded-jacobi-identity.md) with $P_\mu,Q_\alpha,Q_\beta$, using their zero same-chirality anticommutator, then forces $a=0$. Thus the part of the [Super-Poincaré algebra](../../../../../../super-poincare-algebra.md) involving the odd generators is

$$
\boxed{\begin{gathered}
\{Q_\alpha,\bar Q_{\dot\beta}\}=2\sigma^\mu_{\alpha\dot\beta}P_\mu,\qquad\{Q_\alpha,Q_\beta\}=\{\bar Q_{\dot\alpha},\bar Q_{\dot\beta}\}=0,\\
[P_\mu,Q_\alpha]=[P_\mu,\bar Q_{\dot\alpha}]=0.
\end{gathered}}
$$

The last identity means that a supercharge preserves momentum and mass.

The remaining odd-generator commutators express their spinor transformation under rotations and boosts. One consistent lower-index component convention is

$$
\begin{aligned}
[J_i,Q_\alpha]&=-\tfrac12(\sigma_i)_\alpha{}^\beta Q_\beta,&[K_i,Q_\alpha]&=\tfrac i2(\sigma_i)_\alpha{}^\beta Q_\beta,\\
[J_i,\bar Q_{\dot\alpha}]&=\tfrac12(\sigma_i^*)_{\dot\alpha}{}^{\dot\beta}\bar Q_{\dot\beta},&[K_i,\bar Q_{\dot\alpha}]&=\tfrac i2(\sigma_i^*)_{\dot\alpha}{}^{\dot\beta}\bar Q_{\dot\beta}.
\end{aligned}
$$

The barred formulas follow by Hermitian conjugation. Component coefficient matrices act in the dual representation; the signs therefore must be kept consistent, as in the [Jacobi sign test for supercharge components](../../../../../../jacobi-sign-test-for-supercharge-components.md).

One can also derive and check the odd brackets directly in [superspace](../../../../../../superspace.md). With [left Grassmann derivatives](../../../../../../left-grassmann-derivative.md), take

$$
P_\mu=-i\partial_\mu,\qquad Q_\alpha=\partial_{\theta^\alpha}+i\sigma^\mu_{\alpha\dot\gamma}\bar\theta^{\dot\gamma}\partial_\mu,\qquad\bar Q_{\dot\beta}=-\partial_{\bar\theta^{\dot\beta}}-i\theta^\gamma\sigma^\mu_{\gamma\dot\beta}\partial_\mu.
$$

The two cross terms in the mixed anticommutator each give $-i\sigma^\mu\partial_\mu$, totaling $2\sigma^\mu P_\mu$. Equal-chirality terms vanish because the Grassmann derivatives anticommute and their coordinate dependence is of opposite chirality. All coefficients are independent of $x$, so the charges commute with translations. This realizes the displayed algebra rather than merely postulating its brackets.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
