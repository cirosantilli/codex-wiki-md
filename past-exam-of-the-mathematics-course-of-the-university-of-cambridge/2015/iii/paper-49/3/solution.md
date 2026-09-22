<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**Independent metric and [Hamiltonian](../../../../../hamiltonian.md) parametrization.** The Lorentzian [Polyakov action](../../../../../polyakov-action.md) is

$$
\boxed{I_{\mathrm P}[X;\gamma]=-\frac T2\int d^2\sigma\,\sqrt{-\gamma}\,
\gamma^{ab}\partial_aX\cdot\partial_bX.}
$$

The [worldsheet metric](../../../../../worldsheet-metric.md) is independent of the embedding. Its equation sets the traceless [worldsheet stress tensor](../../../../../worldsheet-stress-energy-tensor.md) to zero, making the metric locally conformal to the [induced worldsheet metric](../../../../../induced-worldsheet-metric.md); substitution recovers the [Nambu–Goto action](../../../../../nambu-goto-action.md). Eliminating momentum in the [Nambu-Goto phase-space action](../../../../../nambu-goto-phase-space-action.md) instead gives $(\dot X-uX')^2/(2e)-eT^2X'^2/2$. On the positive-lapse branch, choose the independent metric, up to a positive [Weyl transformation](../../../../../weyl-transformation.md), as

$$
\gamma_{ab}=
\begin{pmatrix}u^2-e^2T^2&u\\u&1\end{pmatrix},\qquad
\sqrt{-\gamma}\,\gamma^{ab}=
\begin{pmatrix}
-1/(eT)&u/(eT)\\
u/(eT)&eT-u^2/(eT)
\end{pmatrix}.
$$

Its determinant is $-e^2T^2$. Multiplication by $-T/2$ recovers the reduced density, including the mixed term $-u\,\dot X\cdot X'/e$. This proves the [phase-space identification of the Polyakov metric](../../../../../phase-space-identification-of-the-polyakov-metric.md).

**Conformal gauge and residual coordinate freedom.** In the [Hamiltonian](../../../../../hamiltonian.md) formulation, [conformal gauge](../../../../../conformal-gauge.md) is $e=1/T,u=0$. The equations become $\ddot X-X''=0$, while $\dot X^2+X'^2=0$ and $\dot X\cdot X'=0$ remain as constraints. In the metric formulation, [conformal gauge](../../../../../conformal-gauge.md) is $\gamma_{ab}=e^{2\omega}\eta_{ab}$, or simply $\eta_{ab}$ after fixing [Weyl invariance](../../../../../weyl-transformation.md). The metric parametrization proves these choices equivalent. Gauge-fixing the metric does not discard the [Virasoro constraints](../../../../../virasoro-constraint.md).

With $\sigma^\pm=t\pm\sigma$, independent reparameterizations $\sigma^\pm\mapsto f_\pm(\sigma^\pm)$ multiply the flat metric by a conformal factor. A compensating [Weyl transformation](../../../../../weyl-transformation.md) restores its chosen representative. Infinitesimally the [Conformal Killing equation](../../../../../conformal-killing-equation.md) is $\partial_-c^+=0,\partial_+c^-=0$. These are the [residual conformal transformations](../../../../../residual-conformal-transformation.md) of two-dimensional [Minkowski spacetime](../../../../../minkowski-spacetime.md), with the periodicity conditions appropriate to a closed string.

**Ghost determinant and anomaly.** For gauge conditions $G_A(\phi)=0$, the [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) is the determinant of the linearized variation

$$
M_{AB}=\frac{\delta G_A(\phi^\epsilon)}{\delta\epsilon^B}\bigg|_{\epsilon=0}.
$$

Insert this determinant in the gauge-fixed [path integral](../../../../../path-integral.md) and exponentiate it with anticommuting ghosts and antighosts: the additional action is proportional to $\int b^AM_{AB}c^B$. In metric [gauge fixing](../../../../../gauge-fixing.md), the [trace](../../../../../matrix-trace.md) is removed by [Weyl invariance](../../../../../weyl-transformation.md), and a [worldsheet diffeomorphism](../../../../../worldsheet-diffeomorphism.md) changes the [trace](../../../../../matrix-trace.md)-free metric through

$$
(P_1c)_{ab}=\nabla_ac_b+\nabla_bc_a-\gamma_{ab}\nabla_dc^d.
$$

Consequently $c^a$ is a vector ghost and $b^{ab}$ a symmetric [trace](../../../../../matrix-trace.md)-free antighost. A conventional normalization of the [worldsheet ghost action](../../../../../worldsheet-ghost-action.md) is

$$
\boxed{I_{\mathrm{gh}}=\frac1{2\pi}\int d^2\sigma\,\sqrt{-\gamma}\,
b^{ab}(P_1c)_{ab}.}
$$

A rescaling of the antighost changes only this overall kinetic normalization. In [conformal gauge](../../../../../conformal-gauge.md), after normalizing the chiral fields, the kinetic terms are

$$
I_{\mathrm{gh}}\propto\int d^2\sigma\,
(b_{++}\partial_-c^++b_{--}\partial_+c^-).
$$

The closed-string ghosts are periodic, with independent left and right systems. Their [conformal weights](../../../../../conformal-weight.md) are $2$ for $b$ and $-1$ for $c$, so the supplied [bc ghost system](../../../../../bc-system.md) expression gives $c_{\mathrm{gh}}=-2(6\cdot2^2-6\cdot2+1)=-26$. Each free embedding boson has [central charge](../../../../../central-charge.md) one per chirality. Hence

$$
\boxed{c_{\mathrm{tot}}=D-26,\qquad D=26\text{ for anomaly cancellation}.}
$$

This [central charge of reparameterization ghosts](../../../../../central-charge-of-reparameterization-ghosts.md) cancels the [string conformal anomaly](../../../../../worldsheet-weyl-anomaly.md) in each chirality separately. Having two sectors does not double the required target dimension.

**Channel variables, poles and the vector state.** With particles 1,2 incoming and 3,4 outgoing, the [Mandelstam variables](../../../../../mandelstam-variables.md) are $s=-(p_1+p_2)^2$ and $t=-(p_1-p_3)^2$. They measure squared center-of-mass [energy](../../../../../energy.md) and momentum transfer. In the specified units $\alpha'=1$, the external tachyon mass squared is $-1$, so $s+t+u=-4$.

The [Gamma function](../../../../../gamma-function.md) [residue](../../../../../residue.md) at $-n$ is $(-1)^n/n!$. At $s=n-1$, its argument $-1-s$ varies with the opposite sign to $s$. The [Gamma function recurrence](../../../../../gamma-function-recurrence.md) gives

$$
\frac{\Gamma(-1-t)}{\Gamma(-1-n-t)}
=(-1)^n\prod_{j=2}^{n+1}(t+j).
$$

Thus the [Veneziano amplitude pole residues](../../../../../veneziano-amplitude-pole-residue.md) are

$$
\boxed{s_n=n-1,\quad n=0,1,\ldots,\qquad
\operatorname*{Res}_{s=s_n}A=-\frac1{n!}\prod_{j=2}^{n+1}(t+j).}
$$

For generic fixed $t$ the [simple poles](../../../../../simple-pole.md) are $-1,0,1,\ldots$. A zero of the [residue](../../../../../residue.md) product at an exceptional negative integer $t$ makes the corresponding pole removable. Fixed $t$ must be away from its own channel poles; fixing it at a channel singularity does not give an ordinary finite meromorphic function of $s$.

At $s=0$, the [residue](../../../../../residue.md) is $-(t+2)=-(t-u)/2$. This is proportional to $(p_1-p_2)\cdot(p_3-p_4)$, the contraction of conserved scalar-pair vector currents. Each current is orthogonal to the exchanged momentum because the external masses in its pair are equal. Alternatively, with scattering-angle cosine $z$, one has $t=-2(s/4+1)(1-z)$; at this pole $t+2=2z$, a pure spin-one angular dependence. Therefore

$$
\boxed{\text{The }s=0\text{ pole exhibits a massless spin-one intermediate string state}.}
$$

The [massless vector pole of the Veneziano amplitude](../../../../../massless-vector-pole-of-the-veneziano-amplitude.md) is the massless open-string vector seen in the two-tachyon exchange channel.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
