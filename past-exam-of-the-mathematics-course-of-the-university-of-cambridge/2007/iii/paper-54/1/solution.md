<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the mostly-positive target [Minkowski spacetime](../../../../../minkowski-spacetime.md) metric and a [closed string](../../../../../closed-string.md) coordinate $0\leq\sigma<2\pi$. In [conformal gauge](../../../../../conformal-gauge.md), variation of the [Polyakov action](../../../../../polyakov-action.md) gives $(\partial_\tau^2-\partial_\sigma^2)X^\mu=0$. The compact coordinate, denoted $X^{25}$, can change by $2\pi Rw$ around the [closed string](../../../../../closed-string.md), with $w\in\mathbb Z$. Write $w^\mu=w\delta^{\mu,25}$. Integrating the two chiral wave solutions and expanding their periodic parts gives the [closed-string mode expansion](../../../../../closed-string-mode-expansion.md)

$$
X^\mu=x^\mu+\alpha'p^\mu\tau+Rw^\mu\sigma
+i\sqrt{\frac{\alpha'}2}\sum_{n\ne0}\frac1n
\left(\alpha_n^\mu e^{-in(\tau-\sigma)}+
\widetilde\alpha_n^\mu e^{-in(\tau+\sigma)}\right).
$$

Reality imposes $\alpha_{-n}=(\alpha_n)^*$ and the analogous condition in the other [chirality](../../../../../chirality-physics.md). The classical compact momentum is continuous; quantization of a wavefunction on the circle subsequently gives $p^{25}=n/R$ with $n\in\mathbb Z$. The [momentum and winding modes](../../../../../momentum-and-winding-modes.md) are most conveniently packaged as

$$
p_R=\frac nR-\frac{wR}{\alpha'},\qquad
p_L=\frac nR+\frac{wR}{\alpha'},\qquad
\alpha_0^{25}=\sqrt{\frac{\alpha'}2}p_R,\quad
\widetilde\alpha_0^{25}=\sqrt{\frac{\alpha'}2}p_L.
$$

For noncompact directions both zero modes are $\sqrt{\alpha'/2}\,p^\mu$. Thus the formula includes both independent [string oscillator](../../../../../string-oscillator.md) families and all compact topological sectors.

Define the [worldsheet stress-energy tensor](../../../../../worldsheet-stress-energy-tensor.md) by $\theta_{ab}=-2(-\gamma)^{-1/2}\delta I/\delta\gamma^{ab}$. Its normalization and components are

$$
\theta_{ab}=\frac1{2\pi\alpha'}
\left(\partial_aX\cdot\partial_bX-
\frac12\gamma_{ab}\gamma^{cd}\partial_cX\cdot\partial_dX\right),
\qquad
\theta_{\tau\tau}=\theta_{\sigma\sigma}
=\frac{\dot X^2+X'^2}{4\pi\alpha'},\quad
\theta_{\tau\sigma}=\frac{\dot X\cdot X'}{2\pi\alpha'}.
$$

An overall rescaling of the named [worldsheet stress tensor](../../../../../worldsheet-stress-energy-tensor.md) does not alter its vanishing. Variation of the independent [worldsheet metric](../../../../../worldsheet-metric.md) imposes $\theta_{ab}=0$, equivalently $(\dot X+X')^2=(\dot X-X')^2=0$. These are the [Virasoro constraints](../../../../../virasoro-constraint.md) that restrict the otherwise general wave solution.

The conjugate momentum density is $P_\mu=\dot X_\mu/(2\pi\alpha')$. The gauge-fixed [Hamiltonian](../../../../../hamiltonian.md) generating $\tau$ translation is therefore

$$
H=\int_0^{2\pi}\frac{\dot X^2+X'^2}{4\pi\alpha'}d\sigma
=L_0+\widetilde L_0,
\qquad
L_m=\frac12\sum_{k\in\mathbb Z}\alpha_{m-k}\cdot\alpha_k,
$$

with the analogous tilded generators. In particular, before imposing the [Virasoro constraints](../../../../../virasoro-constraint.md),

$$
H=\frac{\alpha'}2p_{\rm nc}^2+
\frac{\alpha'}2\left(\frac nR\right)^2+
\frac{w^2R^2}{2\alpha'}+N+\widetilde N,
\qquad
N=\sum_{k>0}\alpha_{-k}\cdot\alpha_k.
$$

The target momentum includes its timelike component, so this is not a positive particle-energy formula. On the classical constraint surface the reparameterization [Hamiltonian](../../../../../hamiltonian.md) vanishes; target energy is the separate charge $p^0$. The difference $L_0-\widetilde L_0=0$ imposes the residual spatial constraint.

In the quantum theory the same quadratic expressions require [normal ordering](../../../../../normal-ordering.md): $[\alpha_m^\mu,\alpha_n^\nu]=m\eta^{\mu\nu}\delta_{m+n,0}$ makes different orderings differ by divergent constants. Their regularized finite remainder is the [normal-ordering constant of a string](../../../../../normal-ordering-constant-of-a-string.md), or [string intercept](../../../../../normal-ordering-constant-of-a-string.md). The [Virasoro central extension](../../../../../virasoro-central-extension.md) also appears. In the critical 26-dimensional [bosonic string theory](../../../../../bosonic-string-theory.md), the 24 transverse [string oscillators](../../../../../string-oscillator.md) give one-unit [string intercept](../../../../../normal-ordering-constant-of-a-string.md) in each [chirality](../../../../../chirality-physics.md). For example their regulated chiral vacuum energy is $24\sum_{k>0}k/2=-1$ using [zeta function regularization](../../../../../zeta-function-regularization.md). The physical zero-mode constraints are $(L_0-1)|\Psi\rangle=(\widetilde L_0-1)|\Psi\rangle=0$.

Let $M$ be the mass seen in the remaining 25 noncompact dimensions. Substituting the compact zero modes in these two constraints gives

$$
M^2=p_R^2+\frac4{\alpha'}(N-1)
=p_L^2+\frac4{\alpha'}(\widetilde N-1).
$$

Taking their mean and difference yields

$$
\boxed{M^2=\frac{n^2}{R^2}+\frac{w^2R^2}{\alpha'^2}
+\frac2{\alpha'}(N+\widetilde N-2),\qquad
\widetilde N-N+nw=0.}
$$

This sign of [compact-circle closed-string level matching](../../../../../compact-circle-closed-string-level-matching.md) follows from assigning tildes to the left-moving sector. Under [T-duality](../../../../../t-duality.md), set $R'=\alpha'/R$, $n'=w$, $w'=n$. Then $p_L'=p_L$ and $p_R'=-p_R$, so reversing the compact right-moving [string oscillators](../../../../../string-oscillator.md) implements the transformation while leaving $N,\widetilde N$ unchanged. Both the mass equation and [closed-string level matching](../../../../../closed-string-level-matching.md) are invariant. This proves invariance of the full [closed string](../../../../../closed-string.md) spectrum, including its [string oscillator](../../../../../string-oscillator.md) degeneracies, rather than only the zero-mode contribution.

A [D-brane](../../../../../d-brane.md) with $p$ spatial [worldvolume](../../../../../worldvolume.md) directions, called a D$p$-brane, is a $(p+1)$-dimensional timelike submanifold on which [open string](../../../../../open-string.md) endpoints have [Neumann boundary conditions](../../../../../neumann-boundary-condition.md) tangentially and [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) transversely. Apply [T-duality](../../../../../t-duality.md) to the compact coordinate by $\widetilde X=X_L-X_R$. The differential relations

$$
\partial_\tau\widetilde X=\partial_\sigma X,\qquad
\partial_\sigma\widetilde X=\partial_\tau X
$$

interchange the two endpoint conditions. Consequently a D$p$-brane wrapping the original circle becomes a D$(p-1)$-brane localized on the dual circle. Its compact [Wilson line](../../../../../wilson-line.md) specifies that position. This is [T-duality of D-brane boundary conditions](../../../../../t-duality-of-d-brane-boundary-conditions.md).

**The separated-brane configuration must instead have the circle transverse to the [D-branes](../../../../../d-brane.md).** Two parallel [D-branes](../../../../../d-brane.md) wrapping the same circle cannot be separated along that [worldvolume](../../../../../worldvolume.md) direction. Thus the latter part describes a new orientation, with both endpoints subject to compact [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md). If their positions differ by $L$, an oriented [Open string stretched between D-branes](../../../../../open-string-stretched-between-d-branes.md) has displacement

$$
L_w=L+2\pi Rw,\qquad w\in\mathbb Z.
$$

On $0\leq\sigma\leq\pi$, its compact classical solution has a linear part $y_1+L_w\sigma/\pi$, plus sine modes vanishing at the endpoints. This adds $L_w^2/(4\pi^2\alpha')$ to the [Virasoro generator](../../../../../virasoro-generator.md) zero mode. Thus, for momentum $\mathbf p$ along the [D-branes](../../../../../d-brane.md),

$$
\boxed{E_w^2=\mathbf p^2+\left(\frac{L_w}{2\pi\alpha'}\right)^2+
\frac{N-1}{\alpha'},\qquad
E_{0,w}^2=\left(\frac{L_w}{2\pi\alpha'}\right)^2-\frac1{\alpha'}.}
$$

The second equation is the quantum rest-energy squared of the [string oscillator](../../../../../string-oscillator.md) ground state; the smallest one uses the shortest allowed compact separation $|L_w|$. Classically the straight string energy is $T|L_w|=|L_w|/(2\pi\alpha')$. The quantum ground state is a [tachyon](../../../../../tachyon.md) if $|L_w|<2\pi\sqrt{\alpha'}$, so in that regime it is an instability rather than a state with real rest energy. Dropping the [string intercept](../../../../../normal-ordering-constant-of-a-string.md) would describe the classical stretched string, not its quantum ground state.

The transverse-circle [T-duality](../../../../../t-duality.md) changes these two [D-branes](../../../../../d-brane.md) to D$(p+1)$-branes wrapping the dual circle. Their positions become the eigenvalues $A_i=y_i/(2\pi\alpha')$ of a constant gauge connection. The [Wilson loop](../../../../../wilson-loop.md) phases are $e^{i2\pi R'A_i}=e^{iy_i/R}$. A string connecting [D-brane](../../../../../d-brane.md) $1$ to [D-brane](../../../../../d-brane.md) $2$ has dual compact momentum

$$
p'_{25}=\frac w{R'}+A_2-A_1
=\frac{L+2\pi Rw}{2\pi\alpha'}.
$$

Its momentum contribution to $E^2$ is exactly the former stretching term, including every winding sector. Qualitatively the two geometrically coincident wrapped [D-branes](../../../../../d-brane.md) are distinguished by their [Wilson lines](../../../../../wilson-line.md), and their connecting strings have shifted momentum quantization. This is how [brane separation becomes a Wilson line](../../../../../brane-separation-becomes-a-wilson-line.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
