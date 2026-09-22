<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use an incoming spacelike [momentum transfer](../../../../../momentum-transfer.md) $q$, so the physical absorption process has $p_X=P+q$, $Q^2=-q^2>0$, and $P\cdot q>0$. There is a sign inconsistency in the original PDF: its delta function has $P-p_X-q$, while its positive [Bjorken x](../../../../../bjorken-x.md) definition and target formulas use incoming $q$. With that literal delta function and $x>0$, the final-state invariant would be

$$
p_X^2=(P-q)^2=M^2-Q^2-2P\cdot q=M^2-Q^2(1+1/x),
$$

which becomes negative in the stated high-energy limit and cannot represent a physical hadronic final state. We therefore use $\delta^4(P+q-p_X)$, preserving the printed $x=Q^2/(2P\cdot q)$ and structure-function conventions. Equivalently, keeping an outgoing momentum variable requires reversing the signs in those definitions as well.

Assume an unpolarized target, incoherent scattering from effectively free spin-one-half [partons](../../../../../parton.md), and the [massless collinear parton approximation](../../../../../massless-collinear-parton-approximation.md). In the [Bjorken scaling](../../../../../bjorken-scaling.md) limit, take $Q^2,P\cdot q\to\infty$ at fixed $0<x<1$, neglecting target and quark masses and intrinsic transverse momentum relative to $Q$. Write the incoming struck-quark momentum as $k=\xi P$ in the leading lightlike-reference approximation. Let $f_f(\xi)$ and $\bar f_f(\xi)$ be quark and antiquark [parton distribution functions](../../../../../parton-distribution-function.md), counting all colours. For the naive scaling result also neglect radiative scaling violations; in full QCD these distributions depend logarithmically on the hard scale.

The outgoing struck quark has momentum $k'=k+q$. Its on-shell condition gives

$$
(k+q)^2=2\xi P\cdot q-Q^2=0,\qquad\boxed{\xi=x.}
$$

Average its initial spin and sum its final spin. The [spin-averaged electromagnetic parton tensor](../../../../../spin-averaged-electromagnetic-parton-tensor.md) has numerator

$$
\begin{aligned}
S^{\mu\nu}(k,q)&=\frac12\operatorname{Tr}[\not k\gamma^\mu(\not k+\not q)\gamma^\nu]\\
&=2[k^\mu(k+q)^\nu+k^\nu(k+q)^\mu-g^{\mu\nu}k\cdot q].
\end{aligned}
$$

The supplied three-gamma identity gives this directly: contract its middle index with $(k+q)_\lambda$ and trace with $\not k$; the $\gamma_5$ trace vanishes. Thus no antisymmetric term survives the unpolarized spin average.

Define transverse tensors

$$
T^{\mu\nu}=-g^{\mu\nu}+\frac{q^\mu q^\nu}{q^2},\qquad \widetilde P^\mu=P^\mu-\frac{P\cdot q}{q^2}q^\mu,\qquad \widetilde k^\mu=k^\mu-\frac{k\cdot q}{q^2}q^\mu.
$$

On the cut, $2k\cdot q=Q^2$, so $\widetilde k=k+q/2=\xi\widetilde P$. Expanding the two transverse terms gives

$$
\boxed{S^{\mu\nu}=Q^2T^{\mu\nu}+4\xi^2\widetilde P^\mu\widetilde P^\nu.}
$$

This also explicitly verifies electromagnetic [current conservation](../../../../../conserved-current.md), $q_\mu S^{\mu\nu}=q_\nu S^{\mu\nu}=0$.

The one-particle final-state [Lorentz-invariant phase-space measure](../../../../../lorentz-invariant-phase-space-measure.md) obeys

$$
\int\frac{d^3k'}{(2\pi)^3\,2k'^0}(2\pi)^4\delta^4(k+q-k')=2\pi\delta_+((k+q)^2).
$$

Including the current's charge factor and the given $1/(4\pi)$ normalization, a single quark therefore contributes

$$
w_f^{\mu\nu}(k,q)=\frac{Q_f^2}{2}\delta_+(2k\cdot q-Q^2)S^{\mu\nu}(k,q).
$$

An antiquark has the same unpolarized tensor and the same squared charge $Q_f^2$.

The [parton convolution normalization for a hadronic tensor](../../../../../parton-convolution-normalization-for-a-hadronic-tensor.md) is

$$
W^{\mu\nu}(P,q)\simeq\sum_f\int_0^1\frac{d\xi}{\xi}[f_f(\xi)+\bar f_f(\xi)]w_f^{\mu\nu}(\xi P,q).
$$

The $1/\xi$ is important: the distributions count parton numbers, whereas covariantly normalized one-particle responses carry the state normalization $2k^0$. The incoherent sum of normalized responses is $W/(2P^0)=\sum_f\int d\xi(f_f+\bar f_f)w_f/(2k^0)$; in the collinear frame $k^0=\xi P^0$, giving the factor above. There is no extra colour multiplicity because it is already included in the distributions.

On the physical cut,

$$
\delta(2\xi P\cdot q-Q^2)=\frac1{2P\cdot q}\delta(\xi-x).
$$

Comparing the two transverse coefficients in the [hadronic tensor](../../../../../hadronic-tensor.md) gives, with $n_f=f_f+\bar f_f$,

$$
W_1\simeq\sum_f\frac{Q_f^2Q^2}{4P\cdot q}\frac{n_f(x)}x=\frac12\sum_fQ_f^2n_f(x),\qquad W_2\simeq\sum_f\frac{Q_f^2}{P\cdot q}\,x n_f(x).
$$

Therefore the requested [deep-inelastic structure functions](../../../../../deep-inelastic-structure-function.md) are

$$
\boxed{F_1(x,Q^2)\simeq\frac12\sum_fQ_f^2[f_f(x)+\bar f_f(x)],\qquad F_2(x,Q^2)\simeq x\sum_fQ_f^2[f_f(x)+\bar f_f(x)].}
$$

The notation $f_f$ here is the question's $f$ with its flavour index made explicit. The calculation proves the [Callan-Gross relation](../../../../../callan-gross-relation.md), $F_2=2xF_1$, rather than merely citing it. Finite masses and radiative corrections modify this leading approximation; at leading QCD order the same formulas use scale-dependent [parton distribution functions](../../../../../parton-distribution-function.md).

The [quark number sum rule](../../../../../quark-number-sum-rule.md) follows because a distribution is a number density. Integrating $f_f$ counts quarks and integrating $\bar f_f$ counts antiquarks; their difference is the net conserved flavour charge:

$$
\boxed{\int_0^1[f_f(x)-\bar f_f(x)]dx=N_f.}
$$

Every sea quark-antiquark pair contributes zero to this difference. More formally the flavour-vector charge counts quarks minus antiquarks and has a fixed eigenvalue on the hadron state. Thus $N_f$ is the valence or net quark number, not the total number including the sea.

Use both final assumptions printed in the question: only up/down flavours and no antiquarks. The second does not follow just from restricting the flavour list. Then $\int f_u=N_u$, $\int f_d=N_d$, with squared charges $Q_u^2=4/9$ and $Q_d^2=1/9$. The [proton](../../../../../proton.md) has $(N_u,N_d)=(2,1)$ and the [neutron](../../../../../neutron.md) $(1,2)$. Hence the [valence-only proton and neutron structure-function moments](../../../../../valence-only-proton-and-neutron-structure-function-moments.md) are

$$
\boxed{\int_0^1\frac{dx}{x}F_2^{\rm proton}(x,Q^2)\longrightarrow\frac49\cdot2+\frac19\cdot1=1,\qquad \int_0^1\frac{dx}{x}F_2^{\rm neutron}(x,Q^2)\longrightarrow\frac49\cdot1+\frac19\cdot2=\frac23.}
$$

The integral limits assume the scaling approximation is valid for the indicated weighted moments, for example by [dominated convergence](../../../../../dominated-convergence-theorem.md) of the weighted integrands. The same net-quark sum rule alone would not fix these individual moments in the presence of antiquarks, since $F_2$ involves the sum of quark and antiquark distributions.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
