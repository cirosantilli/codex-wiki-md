<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Here a [nowhere locally homogeneous metric](../../../../../nowhere-locally-homogeneous-metric.md) means a smooth [Riemannian metric](../../../../../riemannian-metric.md) with no nonidentity [local isometry](../../../../../local-isometry.md): an [isometry](../../../../../isometry.md) between open subsets must fix every point of its domain. This is the strong local-rigidity meaning of “bumpy” used in this question, not the different convention about nondegenerate closed [geodesics](../../../../../geodesic.md). [Sunada's local isometry lemma](../../../../../sunada-local-isometry-lemma.md) states that, on a closed [smooth manifold](../../../../../smooth-manifold.md) of [dimension](../../../../../dimension-vector-space.md) at least two, such [Riemannian metrics](../../../../../riemannian-metric.md) form a residual subset of the space of smooth [Riemannian metrics](../../../../../riemannian-metric.md) and are dense in its $C^\infty$ topology. In [dimension](../../../../../dimension-vector-space.md) one this conclusion is false: arclength coordinates give local translations for every [Riemannian metric](../../../../../riemannian-metric.md).

For maps $M^m\to N^n$, the [jet bundle of maps](../../../../../jet-bundle-of-maps.md) $J^k(M,N)$ records the source point, the target value and all derivatives through order $k$. There are $\binom{m+k}{k}$ monomials of total degree at most $k$ in $m$ variables. Hence

$$
\boxed{\dim J^k(M,N)=m+n\binom{m+k}{k}.}
$$

Over $(x,y)\in M\times N$, the value is already fixed, so the fibre has [dimension](../../../../../dimension-vector-space.md)

$$
\boxed{n\left(\binom{m+k}{k}-1\right).}
$$

In local coordinates it is the space of [Taylor series](../../../../../taylor-series.md) coefficients of orders one through $k$, represented by a [direct sum](../../../../../direct-sum.md) of [symmetric powers](../../../../../symmetric-power.md), $\bigoplus_{r=1}^k\operatorname{Sym}^r(T_x^*M)\otimes T_yN$. This [direct sum](../../../../../direct-sum.md) identification is coordinate-dependent for $k>1$: higher derivatives mix with lower ones under nonlinear coordinate changes. Intrinsically, the truncation to order $k-1$ is an [affine bundle](../../../../../affine-bundle.md) modeled on $\operatorname{Sym}^k(T_x^*M)\otimes T_yN$. For $k=1$ the fibre is canonically $\operatorname{Hom}(T_xM,T_yN)$.

For the density assertion as printed, an [isometry](../../../../../isometry.md) $\overline U_i\to\overline U_j$ is a bijective Riemannian [isometry](../../../../../isometry.md). A [localized volume perturbation](../../../../../localized-volume-perturbation.md) suffices; it is not necessary to prove the stronger generic local-rigidity lemma afresh. We take the coordinate-ball basis without repetitions, and each $U_i$ as the interior of its smooth closed-ball closure. Distinct such domains have a nonempty open difference in at least one direction. Indeed, if both were contained in the other's closure, their regular-open property $U=\operatorname{int}\overline U$ would make them equal.

Fix any [Riemannian metric](../../../../../riemannian-metric.md) $g$. If the two domains have unequal volumes, they cannot be isometric, so $g$ already lies in the desired complement. Otherwise, after interchanging the two indices if necessary, choose a nonnegative nonzero [smooth bump function](../../../../../smooth-bump-function.md) $\psi$ supported in $U_i\setminus\overline U_j$, and set

$$
g_\epsilon=e^{2\epsilon\psi}g.
$$

These are positive-definite smooth [Riemannian metrics](../../../../../riemannian-metric.md) tending to $g$ in the $C^\infty$ topology as $\epsilon\to0$. Their [Riemannian volume forms](../../../../../riemannian-volume-form.md) satisfy $dV_{g_\epsilon}=e^{m\epsilon\psi}dV_g$. The [Riemannian metric](../../../../../riemannian-metric.md) and volume on $U_j$ are unchanged, whereas

$$
\left.\frac d{d\epsilon}\operatorname{vol}_{g_\epsilon}(U_i)\right|_{\epsilon=0}
=m\int_{U_i}\psi\,dV_g>0.
$$

For every sufficiently small $\epsilon>0$, the volumes differ. Thus no [isometry](../../../../../isometry.md) of the two closed domains exists, proving

$$
\boxed{\mathcal C\mathcal S_{ij}\text{ is dense in the space of smooth metrics}.}
$$

The volume difference is continuous in the smooth topology, so the unequal-volume [Riemannian metrics](../../../../../riemannian-metric.md) even form an open dense subset of this complement. The regular-open assumption is also needed to justify this literal closed-domain assertion. As written, requiring only that each closure be a closed ball permits two distinct basis members with the same closure. For example in $\mathbb R^m$, adjoin $U=B(0,1)$ and $V=B(0,1)\setminus\{0\}$ to a countable [basis of a topology](../../../../../basis-of-a-topology.md) of coordinate balls. Both are open and both closures are the same closed ball. The identity is an [isometry](../../../../../isometry.md) of those closures for every [Riemannian metric](../../../../../riemannian-metric.md), so the indicated complement is empty. Thus the conclusion needs distinct closures, as in the usual basis of genuine coordinate balls used above. The no-repetitions convention is necessary as well: if the indexed basis repeats a domain, its identity map is always an [isometry](../../../../../isometry.md) and the asserted complement for those two indices is empty. This volume argument concerns [isometries](../../../../../isometry.md) onto the specified whole domains; the stronger assertion excluding arbitrary [local isometries](../../../../../local-isometry.md) is the separate Sunada lemma stated above.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
