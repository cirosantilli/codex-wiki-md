<h1 id="36d/solution">Solution</h1>

↑ **Parent:** [36D](../36d.md)

An affinely parameterized [geodesic](../../../../../geodesic.md) satisfies $\ddot x^a+\Gamma^a_{bc}\dot x^b\dot x^c=0$. With a general regular parameter $\lambda$ it satisfies

$$
\ddot x^a+\Gamma^a_{bc}\dot x^b\dot x^c=f(\lambda)\dot x^a,
$$

where, if $s$ is affine, $f=s''/s'$. Put $u=\log\Omega$. Substituting $\widetilde g_{ab}=e^{2u}g_{ab}$ and $\widetilde g^{ab}=e^{-2u}g^{ab}$ into the [Christoffel symbol](../../../../../christoffel-symbol.md) formula gives

$$
\boxed{\widetilde\Gamma^a_{bc}=\Gamma^a_{bc}+\delta^a_b\partial_cu+\delta^a_c\partial_bu-g_{bc}g^{ad}\partial_du.}
$$

For an affinely parameterized null tangent $k$, contracting the difference with $k^bk^c$ gives $2k(u)k^a$, since $g(k,k)=0$. The same curve therefore satisfies a nonaffine [geodesic equation](../../../../../geodesic-equation.md) in the conformal metric. It becomes affine there after choosing $d\widetilde\lambda/d\lambda=C\Omega^2$, obtained by setting $d\log(d\widetilde\lambda/d\lambda)/d\lambda=2u'$. **Conformal transformations preserve unparameterized [null geodesics](../../../../../null-geodesic.md).**

In two dimensions each antisymmetric index pair of the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) has only one possible independent component, the pair 01. Pair exchange symmetry then leaves just $R_{0101}$. Contracting with the inverse metric gives

$$
R=2(g^{00}g^{11}-(g^{01})^2)R_{0101}
=\boxed{2\det(g^{ab})R_{0101}}.
$$

Choose $u$ solving $\Box u=R/2$, using the granted solvability, and let $\Omega=e^u>0$. The stated conformal transformation formula gives $\widetilde R=0$. The one-component result makes the full curvature zero. A flat Lorentzian metric is locally isometric to [Minkowski spacetime](../../../../../minkowski-spacetime.md): parallel transport on a simply connected small neighbourhood supplies a parallel orthonormal frame, whose closed dual coframe integrates to flat coordinates. This is a local conclusion; vanishing curvature does not supply global Minkowski coordinates on an arbitrary topology.

In local two-dimensional Minkowski coordinates $U=T-X$, $V=T+X$, a regular smooth null curve obeys $U'V'=0$. Its nonzero continuous tangent stays on one of the two null directions locally, hence the curve lies on $U=\mathrm{constant}$ or $V=\mathrm{constant}$, a straight null line. It is a reparameterized [null geodesic](../../../../../null-geodesic.md). Conformal invariance proves that **every regular null curve in the original two-dimensional metric is a [null geodesic](../../../../../null-geodesic.md)**, without requiring global flat coordinates.

For the displayed metric put $u=\log|t|$. When $t>0$, $ds^2=t(-du^2+d\theta^2)$; when $t<0$, $ds^2=|t|(du^2-d\theta^2)$. In both cases the two null families are

$$
\boxed{\theta=\pm\log|t|+\theta_0.}
$$

If $\theta$ is angular, the endpoints $0,2\pi$ are identified and these wind repeatedly around the cylinder as $t\to0$ and as $|t|\to\infty$. To find the original affine behaviour, the Killing momentum $\ell=t\dot\theta$ is constant and the null condition gives $\dot t^2=\ell^2$. A nontrivial null curve has $\ell\ne0$, so $t$ is affine-linear: it reaches the excluded boundary $t=0$ in finite affine time despite infinitely many windings, and reaches $|t|=\infty$ only in infinite affine time.

The metric is already locally flat. For $t>0$, set $T=2\sqrt t\cosh(\theta/2)$, $X=2\sqrt t\sinh(\theta/2)$; for $t<0$ interchange the hyperbolic sine and cosine with $2\sqrt{|t|}$. Both give $ds^2=-dT^2+dX^2$. The angular identification acts as a Lorentz boost, so these are not global single-valued Minkowski coordinates. Constant-$t$ circles are spacelike for $t>0$ and timelike for $t<0$; the negative branch therefore has closed timelike curves, though its null curves continue to change $t$. If the angular endpoints are not identified, the formulas describe the corresponding unwrapped strips instead. This exhibits concretely the local/global qualification in the earlier request.

## ↑ Ancestors (10)

1. [36D](../36d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
