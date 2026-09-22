<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [mass](../../../../../mass.md) statement needs a nonzero [parallel spinor](../../../../../parallel-spinor.md) and an isolated [asymptotically flat spacetime](../../../../../asymptotically-flat-spacetime.md); the zero [spinor](../../../../../spinor.md) solves the equation on every geometry and cannot imply anything about [mass](../../../../../mass.md). Assume the usual complete regular spin initial data and [dominant energy condition](../../../../../dominant-energy-condition.md) used by the [positive energy theorem](../../../../../positive-energy-theorem.md), with the [spinor](../../../../../spinor.md) tending to a nonzero constant $\epsilon_\infty$ at infinity. Let $V^a=\bar\epsilon\gamma^a\epsilon$ be its future causal [Dirac current](../../../../../dirac-current.md).

The [Nester two-form](../../../../../nester-two-form.md) can be written, up to normalization, as

$$
B^{ab}=\bar\epsilon\gamma^{abc}\nabla_c\epsilon
-\overline{\nabla_c\epsilon}\,\gamma^{abc}\epsilon.
$$

It is bilinear in $\epsilon$ and $\nabla\epsilon$. For a spacetime-parallel [spinor](../../../../../spinor.md) it vanishes identically, and hence so does its asymptotic flux. The [ADM boundary term of the Nester two-form](../../../../../adm-boundary-term-of-the-nester-two-form.md) identifies that flux, up to a fixed positive normalization, as

$$
E V_\infty^0-P_iV_\infty^i=0.
$$

The [positive energy theorem](../../../../../positive-energy-theorem.md) gives $E\geq|P|$. Since $V_\infty$ is nonzero future causal, a future timelike ADM momentum would have strictly positive contraction with it. Consequently the ADM momentum is zero or null:

$$
\boxed{M_{\rm ADM}=\sqrt{E^2-|P|^2}=0.}
$$

In a rest frame, when one exists, this immediately says $E=0$. The usual regular asymptotically flat rigidity conclusion also excludes a nontrivial null-momentum configuration and gives flat initial data. This is the spinorial boundary-charge proof, not an inference that every Lorentzian manifold with a [parallel spinor](../../../../../parallel-spinor.md) is flat. Without the asymptotic and global hypotheses the local [spinor](../../../../../spinor.md) equation alone does not define, let alone determine, an ADM [mass](../../../../../mass.md).

For the modified connection, it is important to fix the [Clifford algebra](../../../../../clifford-algebra.md) normalization. Write

$$
\{\gamma_a,\gamma_b\}=2s\,g_{ab}I,\qquad
\gamma_{ab}=\frac12[\gamma_a,\gamma_b],\qquad s>0.
$$

The compatible [spinor curvature identity](../../../../../spinor-curvature-identity.md) is

$$
[\nabla_a,\nabla_b]=\frac1{4s}R_{abcd}\gamma^{cd}.
$$

Indeed, rescaling conventional [gamma matrices](../../../../../gamma-matrices.md) by $\sqrt s$ rescales $\gamma_{ab}$ by $s$, while leaving the geometric spin connection unchanged. Since the connection is torsion-free and $\nabla\gamma=0$, the cross terms cancel in the modified commutator:

$$
[D_a,D_b]\epsilon=
\left(\frac1{4s}R_{abcd}\gamma^{cd}+c^2[\gamma_a,\gamma_b]\right)\epsilon.
$$

Thus the [Killing-spinor integrability with rescaled gamma matrices](../../../../../killing-spinor-integrability-with-rescaled-gamma-matrices.md) equation is

$$
\boxed{(R_{abcd}\gamma^{cd}+8s c^2\gamma_{ab})\epsilon=0.}
$$

A factor of two in the convention for antisymmetrization multiplies the whole zero equation and cannot change this relative coefficient.

The two printed coefficients are consistent with $s=2$, namely $\{\gamma_a,\gamma_b\}=4g_{ab}I$. In that convention the displayed integrability equation becomes $R_{abcd}\gamma^{cd}+16c^2\gamma_{ab}=0$ on each solution. With the customary convention $s=1$, the coefficient is instead $8c^2$, and the final Ricci coefficient below is $-12c^2$. The PDF does not state its Clifford normalization, so these alternatives must be distinguished rather than mixing them.

In four spacetime dimensions the complex Dirac [spinor](../../../../../spinor.md) fibre has dimension four. Four independent solutions of $D\epsilon=0$ span that fibre at every point: a solution vanishing at one point vanishes everywhere by [parallel transport](../../../../../parallel-transport.md). Therefore the integrability matrix annihilates every [spinor](../../../../../spinor.md) and is the zero matrix. The six bivector matrices $\gamma^{cd}$ are linearly independent, as is seen by taking traces against them; their trace pairing is a nondegenerate multiple of the metric on two-forms. Expressing $\gamma_{ab}=g_{ac}g_{bd}\gamma^{cd}$ therefore gives

$$
R_{abcd}=-4s c^2(g_{ac}g_{bd}-g_{ad}g_{bc}).
$$

This proves that [maximal Killing spinors force constant negative curvature](../../../../../maximal-killing-spinors-force-constant-negative-curvature.md), not merely an Einstein [Ricci tensor](../../../../../ricci-tensor.md). Contracting in four dimensions gives

$$
\boxed{R_{ab}=-12s c^2g_{ab}
=\begin{cases}-24c^2g_{ab},&s=2,\\-12c^2g_{ab},&s=1.\end{cases}}
$$

For $s=2$ this is the requested Einstein equation. Since $c>0$, its [Ricci tensor](../../../../../ricci-tensor.md) automatically has rank four; under the maximal-spinor hypothesis the additional rank assumption is redundant. If the stated four-dimensional solution space is interpreted directly as the pointwise kernel of the algebraic integrability equation, the same spanning and trace argument applies.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
