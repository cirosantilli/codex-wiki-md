<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use [Minkowski spacetime](../../../../../minkowski-spacetime.md) with signature $(-,+,\ldots,+)$, and write the [string tension](../../../../../string-tension.md) as $T=1/(2\pi\alpha')$. If $X^\mu(\tau,\sigma)$ is the [string embedding map](../../../../../string-embedding-map.md), its [induced worldsheet metric](../../../../../induced-worldsheet-metric.md) is $\gamma_{ab}=\partial_aX\cdot\partial_bX$. The [Nambu–Goto action](../../../../../nambu-goto-action.md) is

$$
S=-T\int d\tau\,d\sigma\,\sqrt{-\det\gamma}.
$$

The [first variation](../../../../../first-variation.md) uses $\delta\gamma_{ab}=2\partial_{(a}X_\mu\partial_{b)}\delta X^\mu$ and therefore gives

$$
\delta S=-T\int\sqrt{-\gamma}\,\gamma^{ab}\partial_aX_\mu\partial_b\delta X^\mu\,d\tau\,d\sigma.
$$

An [integration by parts](../../../../../integration-by-parts.md) yields the bulk [Nambu–Goto equations of motion](../../../../../nambu-goto-equations-of-motion.md) and the endpoint term:

$$
\boxed{\partial_a\!\left(\sqrt{-\gamma}\,\gamma^{ab}\partial_bX^\mu\right)=0},
\qquad
\Pi^a_\mu=-T\sqrt{-\gamma}\,\gamma^{ab}\partial_bX_\mu,
\qquad
\left.\Pi^\sigma_\mu\delta X^\mu\right|_{\partial\Sigma}=0.
$$

For a [closed string](../../../../../closed-string.md), periodicity cancels the endpoint term. For a freely moving [open string](../../../../../open-string.md), arbitrary endpoint variations require zero momentum flux, which is the [free-end string boundary condition](../../../../../free-end-string-boundary-condition.md).

Choose orthogonal conformal coordinates on the nondegenerate part of the [worldsheet](../../../../../worldsheet.md), so that $\gamma_{\tau\sigma}=0$ and $\gamma_{\tau\tau}+\gamma_{\sigma\sigma}=0$. The [Nambu–Goto equations of motion](../../../../../nambu-goto-equations-of-motion.md) then become a [wave equation](../../../../../wave-equation-split.md), with the accompanying [Virasoro constraints](../../../../../virasoro-constraint.md):

$$
\ddot X-X''=0,\qquad \dot X\cdot X'=0,\qquad \dot X^2+X'^2=0.
$$

Here a dot and a prime mean $\partial_\tau$ and $\partial_\sigma$. The last two equations are essential: a solution of the [wave equation](../../../../../wave-equation-split.md) alone need not be a relativistic [fundamental string](../../../../../fundamental-string.md) motion.

For a free-ended [open string](../../../../../open-string.md), take $0\leq\sigma\leq\pi$ and $a>0$, and set

$$
X^0=a\tau,\qquad X^1=a\cos\sigma\cos\tau,\qquad X^2=a\cos\sigma\sin\tau,
$$

with the other coordinates constant. Every component satisfies the [wave equation](../../../../../wave-equation-split.md), and

$$
\dot X^2=-a^2\sin^2\sigma,\qquad X'^2=a^2\sin^2\sigma,\qquad \dot X\cdot X'=0.
$$

Moreover $X'=0$ at both endpoints, giving the [Neumann boundary condition](../../../../../neumann-boundary-condition.md). At fixed target time $t=a\tau$, the spatial image is the straight segment

$$
\boldsymbol X=r\bigl(\cos(t/a),\sin(t/a)\bigr),\qquad -a\leq r\leq a.
$$

Thus its [angular velocity](../../../../../angular-velocity.md) is $1/a$. The speed at coordinate $r$ is $|r|/a$, so the endpoints have the [null motion of a free string endpoint](../../../../../null-motion-of-a-free-string-endpoint.md). The [induced worldsheet metric](../../../../../induced-worldsheet-metric.md) degenerates there; the conserved densities below have finite limits, so the endpoint degeneracy causes no divergent charge.

In these coordinates $\Pi^{\tau\mu}=T\dot X^\mu$. The [target-space Noether charges of a string](../../../../../target-space-noether-charges-of-a-string.md) give the [energy](../../../../../energy.md), [momentum](../../../../../momentum.md) and [angular momentum](../../../../../angular-momentum.md):

$$
E=\int_0^\pi T\dot X^0\,d\sigma=\pi Ta,\qquad
\boldsymbol P=T\int_0^\pi\dot{\boldsymbol X}\,d\sigma=0,
$$



$$
J_{12}=T\int_0^\pi\left(X^1\dot X^2-X^2\dot X^1\right)d\sigma
=Ta^2\int_0^\pi\cos^2\sigma\,d\sigma=\frac{\pi Ta^2}{2}.
$$

Since this is the [centre-of-momentum frame](../../../../../center-of-momentum-frame.md), the rest [mass](../../../../../mass.md) is $M=E$. Eliminating $a$ proves the [free-ended straight-string Regge relation](../../../../../free-ended-straight-string-regge-relation.md):

$$
\boxed{J=\frac{M^2}{2\pi T}=\alpha'M^2\quad\text{(free-ended open string)}}.
$$

A spacetime [Lorentz transformation](../../../../../lorentz-transformation.md) of the solution changes its frame, not this rest-frame relation.

There is also a folded [closed string](../../../../../closed-string.md) version: use the same formula over $0\leq\sigma\leq2\pi$. The spatial segment is then covered twice, with folds at $\sigma=0,\pi$, and the [closed-string mode expansion](../../../../../closed-string-mode-expansion.md) is periodic. Each charge is twice its [open string](../../../../../open-string.md) value, so

$$
M=2\pi Ta,\qquad J=\pi Ta^2,\qquad
\boxed{J=\frac{M^2}{4\pi T}=\frac{\alpha'M^2}{2}\quad\text{(folded closed string)}}.
$$

The folds also have degenerate induced metric and are understood through the finite canonical densities or a limiting smooth motion. The two classical [Regge trajectories](../../../../../regge-trajectory.md) have different slopes because the [closed string](../../../../../closed-string.md) has two coincident branches. No quantum [string intercept](../../../../../normal-ordering-constant-of-a-string.md) enters this classical calculation.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 67](../../paper-67-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
