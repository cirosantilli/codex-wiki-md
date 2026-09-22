<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fix a smaller angular strip and a momentum ball $B'\Subset B$; the [canonical transformation](../../../../../../canonical-transformation.md) will be defined there and map into the original domain for small $\epsilon$. This domain restriction is natural for a near-identity change of coordinates with a nonzero momentum shift.

First solve the scalar [cohomological equation on a Diophantine torus](../../../../../../cohomological-equation-on-a-diophantine-torus.md)

$$
\mathcal D_\omega u=\langle V\rangle-V,\qquad\langle u\rangle=0.
$$

The preceding result gives a real-analytic periodic $u$ on every smaller strip. We need a near-identity angular [diffeomorphism](../../../../../../diffeomorphism.md) $\chi$ and a constant vector $a$ such that

$$
D\chi(\theta)\,\omega
=\omega+\epsilon\nabla u(\chi(\theta))+a,
\qquad\chi=\mathrm{id}+O(\epsilon),\quad a=O(\epsilon^2).
$$

Here is a complete analytic construction of this [translated conjugacy of a Diophantine vector field](../../../../../../translated-conjugacy-of-a-diophantine-vector-field.md).

Write $w=\epsilon\nabla u$ and, for a current approximation, put

$$
A=D\chi,\qquad e=\mathcal D_\omega\chi-\omega-w\circ\chi-a.
$$

Assume $A$ is close to the identity. For a correction $\Delta\chi=A v$, the linearized defect is

$$
\mathcal D_\omega(Av)-Dw(\chi)Av-\Delta a
=A\mathcal D_\omega v+(De)v-\Delta a.
$$

The identity follows by differentiating the definition of $e$, so the term $(De)v$ already contains the current error. Choose

$$
\Delta a=\langle A^{-1}\rangle^{-1}\langle A^{-1}e\rangle,
\qquad
\mathcal D_\omega v=A^{-1}(\Delta a-e),\qquad\langle v\rangle=0.
$$

The matrix average is invertible near the identity, and the right-hand side has zero mean. The preceding [torus small-divisor estimate](../../../../../../analytic-estimate-for-the-torus-cohomological-equation.md) therefore solves this vector equation componentwise. Update $\chi_+=\chi+Av$, $a_+=a+\Delta a$. The exact new error is

$$
e_+=(De)v-\bigl[w(\chi+Av)-w(\chi)-Dw(\chi)Av\bigr].
$$

It is quadratic in the current defect.

For convergence, reserve a fixed outer strip on which $w$ is analytic and work on shrinking inner strips whose total loss is less than half the starting width. Let $s=n+\tau$ and choose loss parameters $\delta_j=d\,2^{-j}$ with $0<d<1$ small enough that the fixed multiples of these losses used at each stage fit in the reserved total width. The [torus small-divisor estimate](../../../../../../analytic-estimate-for-the-torus-cohomological-equation.md) and [Cauchy estimates](../../../../../../cauchy-estimate.md) give, with constants uniform while $A$ stays close to the identity and $\chi$ remains in the reserved strip,

$$
\|v_j\|\le C\delta_j^{-s}\|e_j\|,\qquad
\|\Delta\chi_j\|_{C^1}\le C\delta_j^{-(s+1)}\|e_j\|,
\qquad\|\Delta a_j\|\le C\|e_j\|,
$$

and

$$
\|e_{j+1}\|\le C\delta_j^{-\mu}\|e_j\|^2,
\qquad\mu=2s+2.
$$

Indeed, the first remainder is bounded using $\|De_j\|\le C\delta_j^{-1}\|e_j\|$, and the second using the uniformly bounded second derivatives of $w$ on the reserved strip. Taking a slightly larger exponent $\mu$ covers all these losses. Start with $\chi_0=\mathrm{id}$ and $a_0=0$, so $e_0=-w=O(\epsilon)$. If a small constant $K$ satisfies $C d^{-\mu}K2^{2\mu}\le1$ and $\|e_0\|\le K$, induction gives $\|e_j\|\le K2^{-2\mu j}$. The estimates on $\Delta\chi_j$ and $\Delta a_j$ are summable. Choosing $\epsilon$ still smaller keeps the derivatives close to the identity and the images inside the reserved strip, closing the induction. The real periodic analytic limits $\chi,a$ solve the conjugacy equation. Since $\langle w\rangle=0$, the very first constant correction is zero; the first new defect is $O(\epsilon^2)$, and the remaining summed constant corrections are $O(\epsilon^2)$. Also the summed change of $\chi$ is $O(\epsilon)$. This proves the claimed estimates as well as existence, without leaving an unsolved linear remainder.

Now set $\eta(x)=\epsilon\nabla u(x)+a$ and define the [symplectic cotangent lift with a closed momentum shift](../../../../../../symplectic-cotangent-lift-with-a-closed-momentum-shift.md)

$$
\boxed{x=\chi(x'),\qquad
 y=\eta(\chi(x'))+D\chi(x')^{-T}y'.}
$$

The [cotangent lift of a diffeomorphism](../../../../../../cotangent-lift-of-a-diffeomorphism.md) is symplectic. Translation by $\eta$ is also symplectic because the one-form $\eta\cdot dx=\epsilon\,du+a\cdot dx$ is closed. The constant term need not be exact on the [flat torus](../../../../../../flat-torus.md); closedness is sufficient. Thus their composition is the required near-identity [canonical transformation](../../../../../../canonical-transformation.md).

Expanding the quadratic kinetic term gives a transformed linear coefficient $D\chi^{-1}(\omega+\eta\circ\chi)$, which is exactly $\omega$ by the conjugacy equation. The constant-in-$y'$ part is

$$
\omega\cdot\eta+\epsilon V+\frac12|\eta|^2
=\epsilon\langle V\rangle+\omega\cdot a+\frac12|\eta|^2,
$$

since $\mathcal D_\omega u=\langle V\rangle-V$. Consequently define

$$
E_\epsilon=\epsilon\langle V\rangle+\omega\cdot a,
\qquad Q_\epsilon(x',y')=
 y'^T D\chi(x')^{-1}D\chi(x')^{-T}y',
$$

and, for $\epsilon\ne0$,

$$
\widetilde V_\epsilon(x')=\frac12\left|\nabla u(\chi(x'))+\frac a\epsilon\right|^2.
$$

In the exact identities, squared Euclidean norms mean the real polynomial $\sum_j v_j^2$, continued bilinearly on complex strips, without complex conjugation. The latter is uniformly bounded and analytic on the retained strip because $a=O(\epsilon^2)$. At $\epsilon=0$ use the identity map, $E_0=0$, and $Q_0=|y'|^2$. We have the **exact requested normal form**

$$
\boxed{H\circ\Phi=E_\epsilon+\omega\cdot y'
+\frac12Q_\epsilon(x',y')+\epsilon^2\widetilde V_\epsilon(x').}
$$

Here $E_\epsilon=O(\epsilon)$, $Q_\epsilon$ is genuinely homogeneous quadratic in $y'$, and its coefficient matrix differs from the identity by $O(\epsilon)$. Thus $|Q_\epsilon-|y'|^2|\le C|\epsilon|\,|y'|^2$. The remainder depends only on the angular coordinate. If the printed final $\widetilde V(x)$ uses the old angle $x$, the same term is $\tfrac12|\nabla u(x)+a/\epsilon|^2$ evaluated at $x=\chi(x')$; this is just the corresponding coordinate convention.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
