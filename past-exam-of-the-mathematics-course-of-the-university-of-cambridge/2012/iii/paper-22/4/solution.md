<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Hermitian metric](../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) on cotangent vectors is the dual metric, and its exterior-power metric is defined on decomposable vectors by the [determinant](../../../../../determinant.md) of their pairwise inner products. Tensor this with the metric on $E$. In a unitary coframe and unitary frame of $E$, the forms obtained by wedging distinct holomorphic and antiholomorphic coframe elements and tensoring with a frame vector form an orthonormal basis. Let $dV=\omega^n/n!$, and use inner products linear in the first variable.

The [bundle-valued conjugate-linear Hodge star](../../../../../bundle-valued-conjugate-linear-hodge-star.md) is characterized by contraction of the $E,E^*$ coefficients in

$$
\boxed{\psi\wedge *_E\eta=(\psi,\eta)\,dV.}
$$

It is conjugate-linear, maps type $(p,q)$ to type $(n-p,n-q)$, and uses the metric identification of $E$ with its dual. For total degree $k=p+q$, the ordinary star-square rule gives

$$
*_{E^*}*_E=(-1)^k\operatorname{id},
$$

where $E^{**}$ is identified with $E$. The conjugate-linear convention is essential for the bidegrees specified here.

If $\psi$ has degree $k-2$ and $\eta$ degree $k$, the even degree of the real form $\omega$ gives

$$
(L\psi,\eta)dV
=\omega\wedge\psi\wedge *_E\eta
=\psi\wedge L*_E\eta.
$$

Since $*_E\Lambda\eta=L*_E\eta$ for $\Lambda\eta=(-1)^k*_{E^*}L*_E\eta$, it follows that **$(L\psi,\eta)=(\psi,\Lambda\eta)$** pointwise. Thus $\Lambda$ is the [adjoint Lefschetz operator](../../../../../adjoint-lefschetz-operator.md).

For holomorphic $E$, $\bar\partial_E$ differentiates coefficients in [holomorphic local frames](../../../../../holomorphic-local-trivialization.md) and uses the [graded Leibniz rule](../../../../../graded-leibniz-rule.md) on forms. Its [bundle-valued Dolbeault adjoint](../../../../../bundle-valued-dolbeault-adjoint.md) is the formal differential operator

$$
\boxed{\bar\partial_E^*=-*_{E^*}\bar\partial_{E^*}*_E.}
$$

It lowers the antiholomorphic degree by one. To verify this on compact $M$, define $\langle\psi,\eta\rangle_{L^2}=\int_M(\psi,\eta)dV$. For $\psi\in A^{p,q-1}(E)$ and $\eta\in A^{p,q}(E)$, Stokes applied to the scalar $(n,n-1)$-form $\psi\wedge *_E\eta$ yields

$$
\int_M\bar\partial_E\psi\wedge *_E\eta
=(-1)^{p+q}\int_M\psi\wedge\bar\partial_{E^*}*_E\eta.
$$

The star-square identity converts the right side into $\langle\psi,\bar\partial_E^*\eta\rangle_{L^2}$. Compactness and absence of boundary remove boundary terms. This establishes the asserted global adjoint relation on smooth sections.

The [Dolbeault Laplacian](../../../../../dolbeault-laplacian.md) $\Delta_{\bar\partial}=BB^*+B^*B$, with $B=\bar\partial_E$, is formally self-adjoint. Consequently the [adjoint of a commutator](../../../../../adjoint-of-a-commutator.md) satisfies

$$
\boxed{[\Delta_{\bar\partial},L]^*
=\Lambda\Delta_{\bar\partial}-\Delta_{\bar\partial}\Lambda
=[\Lambda,\Delta_{\bar\partial}].}
$$

For the $(1,0)$ part $D'$ of the [Chern connection](../../../../../chern-connection.md), the explicit corresponding adjoint is

$$
\boxed{(D')^*=-*_{E^*}D'_{E^*}*_E,}
$$

where $D'_{E^*}$ is the $(1,0)$ part of the dual [Chern connection](../../../../../chern-connection.md). This is the same integration-by-parts formula in holomorphic degree.

Now assume the metric is Kähler. Since $\bar\partial\omega=0$, $B$ commutes with $L$. Taking adjoints proves

$$
\boxed{[\Lambda,B^*]=0.}
$$

The scalar [Kähler identities](../../../../../kahler-identities.md) needed are

$$
[\Lambda,\bar\partial]=-i\partial^*,\qquad
[\Lambda,\partial]=i\bar\partial^*.
$$

They extend to the [bundle-valued Kähler identities](../../../../../bundle-valued-kahler-identities.md)

$$
[\Lambda,B]=-i(D')^*,\qquad
[\Lambda,D']=iB^*.
$$

Here is a local justification of the extension. At any chosen point, take holomorphic normal coordinates for the Kähler metric and a [holomorphic local frame](../../../../../holomorphic-local-trivialization.md) of $E$ with $H=I$ and $\partial H=0$ at that point. This is a [Chern connection in a normal holomorphic frame](../../../../../chern-connection-in-a-normal-holomorphic-frame.md). Such a frame is obtained first by normalizing the metric matrix at the point and then prescribing the [holomorphic local frame](../../../../../holomorphic-local-trivialization.md) change's first derivatives to cancel $A=H^{-1}\partial H$. The first-order operators and their formal adjoints at the point are then the scalar operators acting componentwise. The scalar identities therefore give the two displayed bundle identities there. Since the point was arbitrary, they hold globally.

Let $A=D'$. Its square and $B^2$ vanish, while

$$
AB+BA=\Theta\wedge-
$$

because the [Chern curvature](../../../../../chern-curvature.md) has pure type $(1,1)$. Use the two commutators already proved to calculate

$$
\begin{aligned}
[\Lambda,\Delta_{\bar\partial}]
&=[\Lambda,B]B^*+B^*[\Lambda,B]\\
&=-i(A^*B^*+B^*A^*)
=-i(\Theta\wedge-)^*.
\end{aligned}
$$

Taking adjoints, including conjugation of the scalar $-i$, gives the [Lefschetz-Dolbeault curvature commutator](../../../../../lefschetz-dolbeault-curvature-commutator.md)

$$
\boxed{[\Delta_{\bar\partial},L]=i\,\Theta\wedge-,
\qquad [L,\Delta_{\bar\partial}]=-i\,\Theta\wedge-.}
$$

If $\Theta=0$, commutation follows. Conversely, vanishing of the commutator on all $E$-valued forms implies $\Theta\wedge s=0$ for every smooth [section of a vector bundle](../../../../../section-of-a-vector-bundle.md) $s$. At any point, a bump-supported local section can have any prescribed fiber value. Thus $\Theta$ annihilates every vector in every fiber, forcing **$\Theta=0$ identically**. This proves the [flatness criterion from Lefschetz commutation](../../../../../flatness-criterion-from-lefschetz-commutation.md); the test on degree-zero forms is why the assertion is made on the entire form space.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
