<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For bosonic embedding coordinates $X^M(\sigma)$, the [supermembrane action](../../../../../supermembrane-action.md) truncates to

$$
\boxed{S=-T_2\int d^3\sigma\,\sqrt{-\det h}
+\frac{qT_2}{3!}\int d^3\sigma\,\varepsilon^{ijk}
\partial_iX^M\partial_jX^N\partial_kX^P A_{MNP}(X),\qquad
h_{ij}=\partial_iX^M\partial_jX^NG_{MN}.}
$$

The first term is its induced [worldvolume](../../../../../worldvolume.md) volume and the second is its [Wess-Zumino brane coupling](../../../../../wess-zumino-brane-coupling.md). A membrane of the opposite orientation reverses $q$.

The [M2-brane supergravity solution](../../../../../m2-brane-supergravity-solution.md) admits the [harmonic function](../../../../../harmonic-function.md)

$$
H(y)=1+\sum_a\frac{Q_a}{|y-y_a|^6},\qquad Q_a>0,
$$

with arbitrary centre positions $y_a$ in eight transverse dimensions. Away from the sources, the [Laplacian](../../../../../laplacian.md) of each term is zero. The unrestricted positions describe static separated membranes carrying aligned charges, so their separations have no potential. Physically, their gravitational attraction is cancelled by their four-form charge repulsion. This is the [M2-brane probe no-force identity](../../../../../m2-brane-probe-no-force-identity.md), which can also be checked directly without relying only on the existence of the multicentre solution.

Keep the field-strength ordering printed in the paper and use $F=dA$. If $\operatorname{vol}_{012}=dx^0\wedge dx^1\wedge dx^2$, a gauge vanishing at infinity is

$$
A=(1-H^{-1})\operatorname{vol}_{012},\qquad
 dA=\operatorname{vol}_{012}\wedge dH^{-1}.
$$

The last equality uses the sign acquired by moving a one-form past a three-form. For this convention the parallel probe has $q=-1$. In [static gauge](../../../../../static-gauge.md), at a fixed transverse position, its [induced worldvolume metric](../../../../../induced-worldvolume-metric.md) is $h_{ij}=H^{-2/3}\eta_{ij}$, hence $\sqrt{-\det h}=H^{-1}$ and

$$
\boxed{\mathcal L_{\mathrm{parallel}}=-T_2H^{-1}-T_2(1-H^{-1})=-T_2,
\qquad\nabla_yV_{\mathrm{parallel}}=0.}
$$

Using the opposite convention for $F$, $A$ and orientation together yields the same cancellation. Changing only the probe charge produces an anti-membrane, with nonconstant potential $T_2(2H^{-1}-1)$. Thus the orientation cannot be dropped from the argument.

The cancellation also survives an expansion for slow transverse motion. With $v^2=|\dot y|^2$,

$$
\mathcal L=-T_2H^{-1}\sqrt{1-Hv^2}-T_2(1-H^{-1})
=-T_2+\frac{T_2}{2}v^2+O(Hv^4).
$$

There is no static potential and no position dependence in the leading kinetic coefficient.

Near an isolated positive membrane charge, write $H\sim R^6/r^6$ with $r=|y-y_a|$ and $R^6=Q_a$. The regular membrane [near-horizon limit](../../../../../near-horizon-limit.md) removes the asymptotically flat constant and gives

$$
ds^2=\frac{r^4}{R^4}\eta_{\mu\nu}dx^\mu dx^\nu
+R^2\frac{dr^2}{r^2}+R^2d\Omega_7^2.
$$

Set $z=R^3/(2r^2)$. Then

$$
\boxed{ds^2=\frac{(R/2)^2}{z^2}
\left(\eta_{\mu\nu}dx^\mu dx^\nu+dz^2\right)+R^2d\Omega_7^2,
\qquad\text{geometry }\mathrm{AdS}_4(R/2)\times S^7(R).}
$$

Thus the [Anti-de Sitter spacetime](../../../../../anti-de-sitter-spacetime.md) radius is half the sphere radius. In orthonormal units the four-form has magnitude $|F|=6/R$ along the AdS volume form, the [Freund-Rubin compactification](../../../../../freund-rubin-compactification.md) flux.

The full asymptotically flat solution has spinors $\epsilon=H^{-1/6}\epsilon_0$ subject to one oriented membrane projector, leaving sixteen real parameters. In the throat, the [Killing spinor](../../../../../killing-spinor.md) equation separates into the standard AdS and sphere equations with correlated signs fixed by the flux. There are four real AdS$_4$ solutions and eight real $S^7$ solutions for the required signs, so

$$
\boxed{N_{\mathrm{susy}}=4\times8=32.}
$$

This is [maximal supersymmetry of AdS4 times S7](../../../../../maximal-supersymmetry-of-ads4-times-s7.md): the additional sixteen spinors need not extend through the asymptotically flat region. A multicentre geometry therefore remains globally sixteen-supersymmetric even though each regular local throat has this enhancement. The classical supergravity description is controlled when $R$ is large compared with the eleven-dimensional [Planck length](../../../../../planck-length.md); singular harmonic multipoles not representing regular positive membrane centres do not automatically have the same throat.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
