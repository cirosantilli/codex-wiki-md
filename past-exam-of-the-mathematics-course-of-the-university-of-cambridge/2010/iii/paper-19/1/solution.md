<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

We use $\Delta=\operatorname{div}\nabla$, whose [spectrum](../../../../../spectrum-functional-analysis.md) on a [compact manifold](../../../../../compact-manifold.md) is nonpositive; write $P=-\Delta$ for the [positive Laplace-Beltrami operator](../../../../../positive-laplace-beltrami-operator.md). This convention will also make the [heat operator](../../../../../heat-operator.md) in Question 3 equal to $\partial_t-\Delta$.

Let $e_1,\ldots,e_d$ be an [orthonormal basis](../../../../../orthonormal-basis.md) of $T_pM$, and let $\gamma_i$ be the unit-speed [geodesic](../../../../../geodesic.md) with $\gamma_i(0)=p$ and $\dot\gamma_i(0)=e_i$. Since a [geodesic](../../../../../geodesic.md) has vanishing acceleration for the [Levi-Civita connection](../../../../../levi-civita-connection.md), differentiation twice along it gives the [Riemannian Hessian](../../../../../riemannian-hessian.md):

$$
\left.\frac{d^2}{dt^2}f(\gamma_i(t))\right|_{t=0}
=\operatorname{Hess}_g f(e_i,e_i).
$$

Taking its [metric trace](../../../../../metric-trace.md) yields the [geodesic trace formula for the Laplace-Beltrami operator](../../../../../geodesic-trace-formula-for-the-laplace-beltrami-operator.md)

$$
\boxed{\Delta f(p)=\sum_{i=1}^d\left.\frac{d^2}{dt^2}f(\gamma_i(t))\right|_{t=0}.}
$$

The positive-sign convention $P$ puts a minus sign in front of this sum.

For the unit [sphere](../../../../../sphere.md), take $p\in S^d$ and tangent unit vectors $e_i$ orthogonal to $p$. Its [great circle](../../../../../great-circle.md) [geodesics](../../../../../geodesic.md) are $\gamma_i(t)=p\cos t+e_i\sin t$. For a smooth ambient function $F$ near the [sphere](../../../../../sphere.md), the ordinary [chain rule](../../../../../chain-rule.md) gives

$$
\left.\frac{d^2}{dt^2}F(\gamma_i(t))\right|_0
=D^2F_p(e_i,e_i)-DF_p(p).
$$

The ambient [orthonormal basis](../../../../../orthonormal-basis.md) is $e_1,\ldots,e_d,p$. Thus, writing $F_r(p)=\partial_rF(rp)|_{r=1}$ and similarly for $F_{rr}$,

$$
\boxed{\Delta_{S^d}(F|_{S^d})
=(\widetilde\Delta F)|_{S^d}-F_{rr}|_{r=1}-dF_r|_{r=1}.}
$$

This proves the [ambient restriction formula for the spherical Laplacian](../../../../../ambient-restriction-formula-for-the-spherical-laplacian.md) and shows why ambient derivatives normal to the [sphere](../../../../../sphere.md) must be subtracted. The equivalent formula in [spherical coordinates](../../../../../spherical-coordinate-system.md) is

$$
\widetilde\Delta F=F_{rr}+\frac d rF_r+\frac1{r^2}\Delta_{S^d}(F(r,\cdot)).
$$

Let $\mathcal P_\ell$ be the [vector space](../../../../../vector-space-split.md) of [homogeneous polynomials](../../../../../homogeneous-polynomial.md) of degree $\ell$ in $d+1$ variables, and $\mathcal H_\ell=\ker\widetilde\Delta\cap\mathcal P_\ell$ its [harmonic polynomials](../../../../../harmonic-polynomial.md). If $H\in\mathcal H_\ell$, [homogeneous polynomial](../../../../../homogeneous-polynomial.md) scaling gives $H(r\omega)=r^\ell H(\omega)$. Substitution into the [spherical coordinates](../../../../../spherical-coordinate-system.md) formula gives

$$
\boxed{P_{S^d}(H|_{S^d})=\ell(\ell+d-1)H|_{S^d}.}
$$

The restrictions are the degree-$\ell$ [spherical harmonics](../../../../../spherical-harmonic.md). A [homogeneous polynomial](../../../../../homogeneous-polynomial.md) vanishing on the [sphere](../../../../../sphere.md) vanishes on every nonzero ray and hence identically, so restriction is injective on $\mathcal H_\ell$.

We prove the [harmonic decomposition of homogeneous polynomials](../../../../../harmonic-decomposition-of-homogeneous-polynomials.md) that both counts these [eigenfunctions](../../../../../eigenfunction.md) and establishes completeness. For an ambient harmonic [homogeneous polynomial](../../../../../homogeneous-polynomial.md) $H_m$ of degree $m$ and $j\geq1$, the [spherical coordinates](../../../../../spherical-coordinate-system.md) formula gives

$$
\widetilde\Delta(r^{2j}H_m)
=2j(2m+2j+d-1)r^{2j-2}H_m.
$$

For $d\geq1$ its coefficient is nonzero. Inductively assume [homogeneous polynomials](../../../../../homogeneous-polynomial.md) of degree $\ell-2$ have been decomposed into sums of $r^{2j}H_m$. Apply this decomposition to $\widetilde\Delta Q$ for $Q\in\mathcal P_\ell$, and lift each summand by multiplying by $r^2$ and dividing by the displayed nonzero coefficient. The resulting $R\in r^2\mathcal P_{\ell-2}$ satisfies $\widetilde\Delta R=\widetilde\Delta Q$, so $Q-R\in\mathcal H_\ell$. The same coefficient formula shows that no nonzero element of $r^2\mathcal P_{\ell-2}$ can be harmonic. Starting at degrees zero and one therefore proves the direct decomposition

$$
\mathcal P_\ell=\mathcal H_\ell\oplus r^2\mathcal P_{\ell-2}.
$$

Since $\dim\mathcal P_\ell=\binom{\ell+d}{d}$, the [multiplicity](../../../../../multiplicity-mathematics.md) is

$$
\boxed{m_\ell=\binom{\ell+d}{d}-\binom{\ell+d-2}{d},}
$$

where the second term is zero for $\ell<2$.

On $r=1$, iterating the decomposition writes every [polynomial](../../../../../polynomial-split.md) restriction as a finite sum of [spherical harmonics](../../../../../spherical-harmonic.md). The [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md) makes these [polynomial](../../../../../polynomial-split.md) restrictions dense in $C(S^d)$, since coordinate functions separate points and constants are included; they are consequently dense in $L^2(S^d)$. [Integration by parts](../../../../../integration-by-parts.md) makes $P$ symmetric on smooth functions and gives orthogonality between distinct [eigenvalues](../../../../../eigenvalue.md). Normalizing within each finite-dimensional [eigenspace](../../../../../eigenspace.md) gives a complete [orthonormal eigenbasis](../../../../../orthonormal-eigenbasis.md) $Y_{\ell a}$. To check the full operator [spectrum](../../../../../spectrum-functional-analysis.md), let $c_{\ell a}=\langle f,Y_{\ell a}\rangle$. For smooth $f$, [integration by parts](../../../../../integration-by-parts.md) gives the coefficients of $Pf$ as $\lambda_\ell c_{\ell a}$. Therefore finite harmonic partial sums approximate both $f$ and $Pf$ in $L^2$, hence approximate in the [graph norm](../../../../../graph-norm.md). Conversely every coefficient sequence with $\sum_{\ell,a}\lambda_\ell^2|c_{\ell a}|^2<\infty$ is the [graph norm](../../../../../graph-norm.md) limit of its finite harmonic sums. Thus the closure of $P$ has exactly this [operator domain](../../../../../operator-domain.md) and is the real diagonal [self-adjoint operator](../../../../../self-adjoint-operator.md) with entries $\lambda_\ell=\ell(\ell+d-1)$. If $z$ is not one of these entries, the inverse has entries $(\lambda_\ell-z)^{-1}$ and is bounded because $\lambda_\ell\to\infty$. This proves that there are no missing spectral values. The [spectrum of the Laplacian on a sphere](../../../../../spectrum-of-the-laplacian-on-a-sphere.md) is

$$
\boxed{\sigma(P)=\{\ell(\ell+d-1):\ell=0,1,2,\ldots\},}
$$

with the above [multiplicities](../../../../../multiplicity-mathematics.md); for $\Delta$, negate every [eigenvalue](../../../../../eigenvalue.md). For example $S^1$ has [eigenvalues](../../../../../eigenvalue.md) $\ell^2$, with [multiplicities](../../../../../multiplicity-mathematics.md) one at zero and two for $\ell\geq1$, and $S^2$ has [multiplicity](../../../../../multiplicity-mathematics.md) $2\ell+1$. The zero-dimensional sphere consists of two isolated points and has only the zero [eigenvalue](../../../../../eigenvalue.md), with [multiplicity](../../../../../multiplicity-mathematics.md) two.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
