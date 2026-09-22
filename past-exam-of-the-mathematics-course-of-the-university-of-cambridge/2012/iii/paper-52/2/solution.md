<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A stable symmetry-breaking minimum requires $\lambda>0$ and $m^2<0$. Put $v^2=-m^2/\lambda>0$. The common [scalar potential](../../../../../scalar-potential.md) can then be written, up to a constant, as

$$
V=\frac\lambda4(\Phi\cdot\Phi-v^2)^2.
$$

Its minima form the sphere $\Phi\cdot\Phi=v^2$. Choose the vacuum direction $\Phi_0=(0,0,v)^T$. If instead $m^2>0$ with positive $\lambda$, the minimum is at the origin and the assumed nonzero [vacuum expectation value](../../../../../vacuum-expectation-value.md) is not a stable vacuum of these models.

In the ungauged theory, the internal symmetry is global $O(3)$; its connected part is $SO(3)$. Constant [orthogonal](../../../../../orthogonal-vectors.md) transformations preserve both the [kinetic term](../../../../../kinetic-term.md) and the potential. The chosen vacuum is invariant under $O(2)$ acting on its first two components, so the continuous breaking is $SO(3)\to SO(2)$ with two broken generators. The vacuum orientations are genuinely different degenerate global vacua.

The [global triplet scalar symmetry breaking](../../../../../global-triplet-scalar-symmetry-breaking.md) is visible directly in the fluctuation masses. Write $\Phi=(\pi_1,\pi_2,v+h)^T$. The potential Hessian is

$$
\left.\frac{\partial^2V}{\partial\Phi_a\partial\Phi_b}\right|_{\Phi_0}
=(m^2+\lambda v^2)\delta_{ab}+2\lambda\Phi_{0a}\Phi_{0b}
=\operatorname{diag}(0,0,2\lambda v^2).
$$

The quadratic Lagrangian is therefore

$$
\mathcal L_1^{(2)}=\frac12(\partial h)^2+\frac12(\partial\pi_1)^2+\frac12(\partial\pi_2)^2-\frac12(2\lambda v^2)h^2.
$$

**There is one radial scalar of [mass](../../../../../mass.md) $m_h^2=2\lambda v^2=-2m^2$ and two massless [Goldstone bosons](../../../../../goldstone-boson.md).** The two Goldstone modes describe motion tangential to the vacuum sphere. They remain physical, since a global rotation has only constant parameters and cannot remove arbitrary spacetime-dependent fluctuations. All three original real-scalar degrees of freedom remain. Interactions persist: the shifted potential is $V-V_{\min}=\frac\lambda4(2vh+h^2+\pi_1^2+\pi_2^2)^2$, containing cubic and quartic terms. Masslessness of the angular modes is protected by the exact continuous symmetry through Goldstone's theorem.

In the gauged theory, the three-component real field is the vector representation of local $SO(3)$, equivalently the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) of $SU(2)$. The center of $SU(2)$ acts trivially on this field, so both descriptions have the same local field content and perturbative spectrum. Take $(t^a)_{bc}=-i\epsilon^{abc}$, for which $[t^a,t^b]=i\epsilon^{abc}t^c$. The covariant [kinetic term](../../../../../kinetic-term.md) and the gauge [kinetic term](../../../../../kinetic-term.md) are invariant under local transformations with the associated connection transformation. The scalar inversion $\Phi\mapsto-\Phi$, with the [gauge field](../../../../../gauge-field.md) unchanged, is also a discrete invariance of the displayed action.

The vacuum leaves rotations about its third axis unbroken. The residual gauge group is $SO(2)$, or the corresponding $U(1)$ subgroup in the $SU(2)$ description. Expanding the covariant [kinetic term](../../../../../kinetic-term.md) about $\Phi_0$ gives

$$
\frac12(D_\mu\Phi_0)\cdot(D^\mu\Phi_0)
=\frac12g^2v^2\left(B_\mu^1B^{1\mu}+B_\mu^2B^{2\mu}\right).
$$

Thus the [gauge-boson mass matrix](../../../../../gauge-boson-mass-matrix.md) is $g^2v^2\operatorname{diag}(1,1,0)$. The third generator annihilates the vacuum, while the first two do not. **The masses are $m_{B^1}=m_{B^2}=gv$, $m_{B^3}=0$, and $m_h=\sqrt{2\lambda}\,v$.**

The quadratic derivative mixing displays what happens to the Goldstone fields. With the generator convention just chosen,

$$
(D_\mu\Phi)_1=\partial_\mu\pi_1-gvB_\mu^2+\cdots,\quad
(D_\mu\Phi)_2=\partial_\mu\pi_2+gvB_\mu^1+\cdots,\quad
(D_\mu\Phi)_3=\partial_\mu h+\cdots.
$$

Local rotations can set the two angular fields to zero in [unitary gauge](../../../../../unitary-gauge.md). Then $\Phi=(0,0,v+h)^T$ and

$$
\mathcal L_{\rm scalar}=\frac12(\partial h)^2
+\frac12g^2(v+h)^2\left[(B^1)^2+(B^2)^2\right]-V(v+h).
$$

The two Goldstone modes supply the [longitudinal polarizations](../../../../../longitudinal-polarization.md) of the two massive vector bosons. They do not survive as additional physical massless scalars. The radial scalar is still physical, and $B^3$ retains only two [transverse polarizations](../../../../../transverse-polarization.md). This [adjoint triplet Higgs spectrum](../../../../../adjoint-triplet-higgs-spectrum.md) realizes the [Higgs mechanism](../../../../../higgs-mechanism.md); the gauge group is only partially broken, so one massless [gauge boson](../../../../../gauge-boson.md) remains.

The degree-of-freedom check is

$$
\boxed{\text{before: }3+3\times2=9,\qquad
\text{after: }1+2\times3+1\times2=9.}
$$

In contrast, the global theory has just the three scalar modes, including its two physical [Goldstone bosons](../../../../../goldstone-boson.md). A [vacuum expectation value](../../../../../vacuum-expectation-value.md) in the local theory is a choice of gauge-fixed description: the direction can be changed by [gauge transformations](../../../../../gauge-transformation.md) and is not itself an observable. Gauge-independent masses and the physical degree count express the actual effect. Both theories retain Lorentz symmetry in the constant scalar vacuum.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
