<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

First regulate the [Gaussian functional integral](../../../../../gaussian-functional-integral.md), separating any constant zero mode. Integration by parts gives $S[\phi]=\tfrac12(\phi,A\phi)$ with positive kinetic operator $A=-\Delta$ on the nonzero modes. Complete the square:

$$
\frac12(\phi,A\phi)+(J,\phi)
=\frac12(\phi+A^{-1}J,A(\phi+A^{-1}J))-\frac12(J,A^{-1}J).
$$

A translation of the regulated integration variables then yields

$$
Z[J]=\mathcal N\exp\left[\frac12(J,A^{-1}J)\right]
=\boxed{\mathcal N\exp\left[-\frac12(J,GJ)\right]},
\qquad G=-A^{-1}=\Delta^{-1}.
$$

The sign is essential: the kernel in the negative source exponent is the negative of the positive Gaussian covariance. The source-independent prefactor is formally $\mathcal N=\int D\chi\,e^{-(\chi,A\chi)/2}\propto(\det{}'A)^{-1/2}$, with the prime denoting the excluded zero mode and normalization depending on the regulated measure. This is the [Euclidean scalar source functional and Laplacian sign](../../../../../euclidean-scalar-source-functional-and-laplacian-sign.md) convention.

Consequently $\Delta_zG(z,w)=\delta^{(2)}(z-w)$. In the plane,

$$
\boxed{G(z,w)=\frac1{2\pi}\log\frac{|z-w|}{L}}
$$

up to harmonic additions fixed by boundary and infrared conditions. Away from $w$ this logarithm is harmonic. Integrating its outward normal derivative around a small circle centered at $w$ gives $2\pi$, establishing the distributional delta coefficient. The arbitrary infrared length $L$ cancels for a source of zero total integral. On a compact regulated [worldsheet](../../../../../worldsheet.md) the zero-mode-projected equation has the corresponding constant subtraction from the delta function.

For the string action $I_E=(4\pi\alpha')^{-1}\int(\partial X)^2$, the nonzero-mode covariance is

$$
\langle X^\mu(z)X^\nu(w)\rangle_0=-\alpha'\eta^{\mu\nu}\log\frac{|z-w|}{L}.
$$

Compute initially with Euclidean target coordinates and restore target Lorentzian contractions by analytic continuation. Treat the physical [tachyon](../../../../../tachyon.md) vertices as normal-ordered exponentials; this removes coincident self-contractions. Completing the Gaussian square with the imaginary delta-function sources, or applying [Wick contractions](../../../../../wick-contraction.md), gives

$$
\left\langle\prod_{r=1}^4:e^{ik_r\cdot X(z_r)}:\right\rangle_{\rm nonzero}
=\prod_{r<s}|z_r-z_s|^{\alpha'k_r\cdot k_s}
$$

after fixing the vertex normalization. Each cross-contraction has the sign $i^2=-1$, canceling the negative logarithmic covariance, which explains the positive exponent.

The constant target-space mode must also be integrated:

$$
\int d^dx_0\,e^{ix_0\cdot\sum_rk_r}
=(2\pi)^d\delta^{(d)}\!\left(\sum_rk_r\right).
$$

This momentum-conservation factor is momentum dependent and cannot literally be absorbed into the PDF's momentum-independent $\mathcal N$. Its intended position integral is the amplitude with this overall delta function stripped off, restricted to conserving momenta. In that convention,

$$
\boxed{\widehat A_4=\mathcal N\int\prod_{q=1}^4d^2z_q\,
\prod_{r<s}|z_r-z_s|^{\alpha'k_r\cdot k_s}.}
$$

The logarithmic infrared constant only gives a fixed normalization on the common external mass shell, since $\sum_{r<s}k_r\cdot k_s=-\tfrac12\sum_rk_r^2$. Thus the Gaussian determinant and normalization are independent of the scattering invariants. To make the tree position integral finite one also divides by the residual Möbius gauge volume, equivalently fixes three insertions with their ghost factor. The four-position expression is its formal unfixed representation.

Under $z\mapsto(az+b)/(cz+d)$ with determinant one,

$$
z_r'-z_s'=\frac{z_r-z_s}{(cz_r+d)(cz_s+d)},\qquad
 d^2z_r'=|cz_r+d|^{-4}d^2z_r.
$$

At insertion $r$, the [Koba-Nielsen factor](../../../../../koba-nielsen-factor.md) therefore contributes $|cz_r+d|^{-\alpha'\sum_{s\ne r}k_r\cdot k_s}$. [Momentum conservation](../../../../../momentum-conservation.md) makes the exponent $\alpha'k_r^2$. On the [tachyon](../../../../../tachyon.md) mass shell $k_r^2=4/\alpha'$, it is four and cancels the measure's exponent $-4$. Hence **the full integration density is Möbius invariant**. The correlator factor alone is covariant; the density including $d^2z_r$ is invariant.

The supplied [Virasoro–Shapiro amplitude](../../../../../virasoro-shapiro-amplitude.md) has generic simple poles when $-1-\alpha's/4=-n$, giving

$$
\boxed{s=M_n^2=\frac{4(n-1)}{\alpha'},\quad n=0,1,2,\ldots,}
$$

and likewise in the other channels. These are exchanges of closed-string states with equal left and right levels $n$: the [tachyon](../../../../../tachyon.md), the massless sector and the massive tower. At special kinematics zeros or crossed-channel coincidences need to be handled by the full constrained amplitude; numerator poles are not three independent sequences of unrelated singularities.

To isolate the three-tachyon coupling, first use [momentum conservation](../../../../../momentum-conservation.md) and $k_r^2=-\mu^2$:

$$
s+t+u=6\mu^2-2k_1\cdot(k_2+k_3+k_4)
=6\mu^2+2k_1^2=\boxed{4\mu^2}.
$$

At the [tachyon](../../../../../tachyon.md) pole $s=\mu^2=-4/\alpha'$, put $x=\alpha't/4$ and $y=\alpha'u/4$. The relation gives $x+y=-3$. Thus $-1-y=2+x$ and $2+y=-1-x$, and the entire $t,u$ gamma-function ratio cancels to one. The remaining numerator is $\Gamma(-\alpha'(s-\mu^2)/4)\sim-4/[\alpha'(s-\mu^2)]$, while its denominator tends to $\Gamma(1)=1$. Hence

$$
\boxed{\widehat A_4\sim\frac{4C/\alpha'}{\mu^2-s},
\qquad\operatorname*{Res}_{s=\mu^2}\widehat A_4=-\frac{4C}{\alpha'}.}
$$

With the exchange convention $\widehat A_4\sim g_{TTT}^2/(\mu^2-s)$ and canonically normalized external legs, factorization therefore gives $\boxed{g_{TTT}^2=4C/\alpha'}$, or $g_{TTT}=2\sqrt{C/\alpha'}$ up to its unobservable overall sign. A convention using the opposite propagator denominator or factors of $i$ changes the corresponding amplitude phase. Because $C$ itself is unspecified, the residue fixes this relation, not an absolute numerical coupling independent of normalization.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
