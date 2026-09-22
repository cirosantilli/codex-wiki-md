<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

First fix the photon momentum convention. With $Q^2=-q^2>0$, $\nu=P\cdot q>0$ and $x=Q^2/(2\nu)>0$, an absorbed photon gives final momentum $p_X=P+q$. This is the [physical momentum support of a deep-inelastic hadronic tensor](../../../../../physical-momentum-support-of-a-deep-inelastic-hadronic-tensor.md). The original PDF instead prints $\delta^{(4)}(P-p_X-q)$ while keeping that positive-$x$ convention. Taken literally, it would require

$$
p_X^2=(P-q)^2=M^2-Q^2(1+1/x)<0
$$

in the [Bjorken scaling](../../../../../bjorken-scaling.md) limit, leaving no physical final states. The sign is therefore inconsistent with the requested nonzero [deep-inelastic structure functions](../../../../../deep-inelastic-structure-function.md). Below, use the physically consistent absorption delta function $\delta^{(4)}(P+q-p_X)$. Alternatively all photon-momentum and scaling-variable conventions would have to be reversed together.

Work in the leading [parton model](../../../../../parton-model.md): the target is unpolarized; scattering is incoherent from massless collinear [quarks](../../../../../quark.md) and [antiquarks](../../../../../antiquark.md); intrinsic transverse momentum and target-mass effects are neglected. The [parton distribution functions](../../../../../parton-distribution-function.md) count constituents and include their colour multiplicity. At this order, neglect strong radiative corrections and the resulting logarithmic scale evolution.

Let a quark carry momentum $p=\xi P$, using a lightlike reference $P$ at leading order, and let $r=p+q$. The spin-averaged electromagnetic trace is

$$
\frac12\operatorname{tr}(\not p\gamma^\mu\not r\gamma^\nu)=2[p^\mu r^\nu+p^\nu r^\mu-g^{\mu\nu}p\cdot r].
$$

Integrating its one-particle final [Lorentz-invariant phase space](../../../../../lorentz-invariant-phase-space.md), with the $1/(4\pi)$ tensor normalization, supplies $\delta_+(r^2)/2$. Thus the [spin-averaged electromagnetic parton tensor](../../../../../spin-averaged-electromagnetic-parton-tensor.md) is

$$
w_f^{\mu\nu}=Q_f^2\delta_+(r^2)[p^\mu r^\nu+p^\nu r^\mu-g^{\mu\nu}p\cdot r].
$$

On physical support, $r^2=0$ gives $\xi=x$ and $p\cdot q=Q^2/2$. Define the transverse tensors

$$
t^{\mu\nu}=-g^{\mu\nu}+q^\mu q^\nu/q^2,\qquad \widetilde P^\mu=P^\mu-(\nu/q^2)q^\mu.
$$

The bracket in $w_f$ becomes

$$
\frac{Q^2}{2}t^{\mu\nu}+2\xi^2\widetilde P^\mu\widetilde P^\nu.
$$

This follows by writing $p=\xi\widetilde P-q/2$ on shell and expanding; it also verifies transversality to $q$.

The correct [parton convolution normalization for a hadronic tensor](../../../../../parton-convolution-normalization-for-a-hadronic-tensor.md) is

$$
W^{\mu\nu}=\sum_f\int_0^1\frac{d\xi}{\xi}[q_f(\xi)+\bar q_f(\xi)]w_f^{\mu\nu}(\xi P,q).
$$

The $1/\xi$ converts number weighting into covariant target-state normalization: a parton response per constituent is normalized by $2p^0$, whereas the hadron tensor uses $2P^0$, and $P^0/p^0=1/\xi$. Antiquark charge changes sign but its square and symmetric spin trace are the same.

Use the [parton on-shell delta identity](../../../../../parton-on-shell-delta-identity.md),

$$
\delta(r^2)=\delta(2\nu(\xi-x))=\frac{\delta(\xi-x)}{2\nu}.
$$

Matching the two tensor coefficients now gives

$$
\boxed{F_1=W_1=\frac12\sum_fQ_f^2[q_f(x)+\bar q_f(x)],\qquad F_2=\nu W_2=x\sum_fQ_f^2[q_f(x)+\bar q_f(x)].}
$$

In particular $F_2=2xF_1$, the [Callan-Gross relation](../../../../../callan-gross-relation.md) for spin-one-half partons. Scaling here means the naive leading approximation; full [Quantum chromodynamics](../../../../../quantum-chromodynamics.md) produces scale-dependent distributions and corrections.

Each [quark](../../../../../quark.md) contributes $+1$ and each [antiquark](../../../../../antiquark.md) contributes $-1$ to its flavour-vector charge. Sea pairs therefore cancel in the [quark number sum rule](../../../../../quark-number-sum-rule.md):

$$
\boxed{\int_0^1[q_f(x)-\bar q_f(x)]\,dx=N_f.}
$$

Here $N_f$ is the net flavour number, not the total number including sea pairs. This condition by itself fixes no antiquark distribution.

Under the separately imposed valence-only approximation, $\bar q_f=0$ and only up/down distributions remain. The [proton](../../../../../proton.md) has $(N_u,N_d)=(2,1)$ and the [neutron](../../../../../neutron.md) has $(1,2)$. With $Q_u=2/3$, $Q_d=-1/3$, the [valence-only proton and neutron structure-function moments](../../../../../valence-only-proton-and-neutron-structure-function-moments.md) are

$$
\boxed{\int_0^1\frac{F_2^p(x)}x\,dx=\frac49(2)+\frac19(1)=1,\qquad \int_0^1\frac{F_2^n(x)}x\,dx=\frac49(1)+\frac19(2)=\frac23.}
$$

No extra factor of three belongs here: colour is already included in the constituent distributions and the flavour counts. These are conditional valence-model moments, not unrestricted asymptotic statements in a theory whose evolution generates a sea.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
