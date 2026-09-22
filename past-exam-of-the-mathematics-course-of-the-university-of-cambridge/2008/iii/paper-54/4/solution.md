<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The last panel of the preceding process figure shows [deep inelastic scattering](../../../../../deep-inelastic-scattering.md) through a virtual [photon](../../../../../photon.md). The blob represents the electromagnetic [hadronic tensor](../../../../../hadronic-tensor.md) response, with all final hadronic states included. With charges factored into $e$ and the hadronic current as in the question, a suitable [scattering amplitude](../../../../../scattering-amplitude.md), up to an irrelevant overall phase, is

$$
\boxed{\mathcal M_X=\frac{e^2}{Q^2}\overline u(p')\gamma_\mu u(p)
\langle X|J_h^\mu|H(P)\rangle,\qquad Q^2=-q^2.}
$$

The electron [fermion spin sum](../../../../../fermion-spin-sum.md), before averaging the two initial spin states, gives the following normalization of the [leptonic tensor](../../../../../leptonic-tensor.md):

$$
\boxed{L_{\mu\nu}=\operatorname{Tr}[\not p'\gamma_\mu\not p\gamma_\nu]
=4(p'_\mu p_\nu+p'_\nu p_\mu-g_{\mu\nu}p\cdot p').}
$$

The initial electron spin average is a separate factor $1/2$. Equivalently one can absorb it into a tensor $L/2$, but the prefactor in the requested formula uses the unaveraged trace $L$. The massless Dirac equations imply $q^\mu L_{\mu\nu}=q^\nu L_{\mu\nu}=0$, the relevant [Ward identity](../../../../../ward-identity.md).

In the target rest frame the incident flux is $4p\cdot P=4ME$. This remains valid for a massive target because the electron is massless: the general flux $4\sqrt{(p\cdot P)^2-p^2P^2}$ reduces to that expression. The outgoing electron contributes $d^3p'/((2\pi)^3 2E')$, and the inclusive final-state sum is $4\pi W_H^{\mu\nu}$. Including the electron spin average therefore gives

$$
\begin{aligned}
\frac{d\sigma}{d^3p'}
&=\frac{1}{4ME}\frac{1}{(2\pi)^3 2E'}\frac{e^4}{(Q^2)^2}
\frac12L_{\mu\nu}(4\pi W_H^{\mu\nu})\\
&=\boxed{\frac{e^4}{(2\pi)^2\,8MEE'(Q^2)^2}
L_{\mu\nu}W_H^{\mu\nu}.}
\end{aligned}
$$

The implicit hadron spin average in $W_H$ must not be inserted a second time.

For an unpolarized target, [Lorentz invariance](../../../../../lorentz-invariance.md) permits tensor structures formed from $P$, $q$ and the metric. Hermiticity relates the two index orders. The electromagnetic response is parity even, excluding the pseudotensor $i\epsilon^{\mu\nu\rho\sigma}P_\rho q_\sigma$. A possible ordinary antisymmetric $P^\mu q^\nu-q^\mu P^\nu$ term is excluded by [current conservation](../../../../../conserved-current.md). The symmetric part initially has four structures, $g^{\mu\nu}$, $P^\mu P^\nu$, $q^\mu q^\nu$ and $P^\mu q^\nu+q^\mu P^\nu$. Imposing both current-conservation conditions leaves the [transverse decomposition of an unpolarized hadronic tensor](../../../../../transverse-decomposition-of-an-unpolarized-hadronic-tensor.md):

$$
W_H^{\mu\nu}=-\left(g^{\mu\nu}-\frac{q^\mu q^\nu}{q^2}\right)F_1
+\left(P^\mu-\frac{\nu}{q^2}q^\mu\right)
 \left(P^\nu-\frac{\nu}{q^2}q^\nu\right)\frac{F_2}{\nu},
\qquad\nu=P\cdot q.
$$

For example, contracting $q$ into the first structure gives $(1+A)q^\mu$ in the printed parametrization, and contracting into either parenthesis gives $(1+B)\nu$ or $(1+C)\nu$. Since the two independent [deep-inelastic structure functions](../../../../../deep-inelastic-structure-function.md) are not generally linked by symmetry, transversality requires

$$
\boxed{A=B=C=-1.}
$$

There are only two invariant variables once $P^2=M^2$ is fixed; they may be chosen as $Q^2$ and [Bjorken x](../../../../../bjorken-x.md) $x=Q^2/(2\nu)$.

Now make the leading [massless collinear parton approximation](../../../../../massless-collinear-parton-approximation.md). In the hard parton calculation, use a lightlike collinear reference for $P$, neglecting target-mass effects of relative order $M^2/Q^2$ as well as quark masses. Literally combining a massive $P$ with an exactly massless constituent momentum $\xi P$ would be inconsistent. The exact rest-frame flux derived above does not require this approximation; it is the following partonic response that does.

Let $r=\xi P$ and $k=r+q$. Strip the quark charge out of the current, since its square is already the factor $Q_f^2$ in the parton convolution. Averaging the initial quark spin and summing the final spin gives the [spin-averaged electromagnetic parton tensor](../../../../../spin-averaged-electromagnetic-parton-tensor.md)

$$
S^{\mu\nu}=\frac12\operatorname{Tr}[\not r\gamma^\nu\not k\gamma^\mu]
=2(r^\mu k^\nu+r^\nu k^\mu-g^{\mu\nu}r\cdot k).
$$

The spatial momentum delta fixes $\boldsymbol k=\boldsymbol q+\xi\boldsymbol P$. The remaining one-particle [Lorentz-invariant phase space](../../../../../lorentz-invariant-phase-space.md), together with $1/(4\pi\xi)$ in the definition, supplies

$$
\frac{1}{4\pi\xi}\frac{(2\pi)^4}{(2\pi)^3\,2E_k}
\delta(E_q+\xi E_P-E_k)=\frac{\delta(E_q+\xi E_P-E_k)}{4\xi E_k}.
$$

Since $r^2=k^2=0$ and $r\cdot k=\xi P\cdot q$, the full parton response is

$$
\widetilde W^{\mu\nu}=\frac{\delta(E_q+\xi E_P-E_k)}{E_k}
\left[\xi P^\mu P^\nu+\frac{P^\mu q^\nu+q^\mu P^\nu}{2}
-\frac{\nu}{2}g^{\mu\nu}\right].
$$

Terms with a free $q$ index vanish when contracted with the conserved [leptonic tensor](../../../../../leptonic-tensor.md). Thus **the part of $\widetilde W$ contributing to the cross-section is**

$$
\boxed{\widetilde W^{\mu\nu}\ \doteq\
\frac{\delta(E_q+\xi E_P-E_k)}{E_k}
\left[\xi P^\mu P^\nu-\frac{\nu}{2}g^{\mu\nu}\right],}
$$

where $\doteq$ denotes equality in that contraction, rather than an equality of the full tensors. The omitted terms are necessary for the full [hadronic tensor](../../../../../hadronic-tensor.md) to be transverse; the wording about contributing terms in the PDF is important here.

To prove the delta identity with the correct Jacobian, set $\omega=E_q+\xi E_P$. On physical support $E_k>0$ and $\omega>0$. Factoring $E_k^2-\omega^2=(E_k-\omega)(E_k+\omega)$ gives the [positive-energy on-shell delta function identity](../../../../../positive-energy-on-shell-delta-function-identity.md)

$$
\frac{\delta(\omega-E_k)}{E_k}=2\delta(E_k^2-\omega^2).
$$

This is restricted to the positive-energy branch; the other root must not be included. Using the spatial momentum constraint and $P^2=0$ in the leading hard approximation,

$$
E_k^2-\omega^2=-(q+\xi P)^2=Q^2-2\xi\nu=2\nu(x-\xi).
$$

The [Dirac delta function](../../../../../dirac-delta-function.md) change of variable therefore gives the [parton on-shell delta identity](../../../../../parton-on-shell-delta-identity.md)

$$
\boxed{\frac{\delta(E_q+\xi E_P-E_k)}{E_k}
=2\delta(E_k^2-(E_q+\xi E_P)^2)
=\frac{\delta(x-\xi)}{\nu}.}
$$

Here $\nu>0$. This is the actual printed identity: the converted TeX's final $\delta(x)/E_k$ is a transcription error. If target mass is formally retained in the delta argument, it becomes $Q^2-2\xi\nu-\xi^2M^2$, so the stated simple root and Jacobian no longer apply.

Let $D(x)=\sum_fQ_f^2(q_f(x)+\overline q_f(x))$. The parton integral collapses at $\xi=x$, giving

$$
W_H^{\mu\nu}\doteq D(x)\left[\frac{x}{\nu}P^\mu P^\nu-\frac12g^{\mu\nu}\right].
$$

The [transverse decomposition of an unpolarized hadronic tensor](../../../../../transverse-decomposition-of-an-unpolarized-hadronic-tensor.md), in the same contraction, is $-g^{\mu\nu}F_1+P^\mu P^\nu F_2/\nu$. Comparing the two independent structures yields

$$
\boxed{F_1(x,Q^2)=\tfrac12D(x),\qquad F_2(x,Q^2)=xD(x),\qquad
F_2=2xF_1.}
$$

This derives the [Callan-Gross relation](../../../../../callan-gross-relation.md) from the spin-one-half trace and on-shell constraint. Antiquarks give the same symmetric response and therefore the sum $q_f+\overline q_f$. The result applies at leading order in the massless [parton model](../../../../../parton-model.md); target masses, intrinsic transverse momentum and [Quantum chromodynamics](../../../../../quantum-chromodynamics.md) radiative effects can generate a nonzero [longitudinal deep-inelastic structure function](../../../../../longitudinal-deep-inelastic-structure-function.md) and modify the relation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
