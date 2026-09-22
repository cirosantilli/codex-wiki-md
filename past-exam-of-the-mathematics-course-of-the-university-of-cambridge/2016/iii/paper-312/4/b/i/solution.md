<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Distinguish the [slow-roll approximation](../../../../../../../slow-roll-approximation.md) parameter $\epsilon$ from the infinitesimal positive contour regulator $\varepsilon$. In the [interaction picture](../../../../../../../interaction-picture.md), the ordered unequal-time [Wick contraction](../../../../../../../wick-contraction.md) is

$$
\langle\zeta(\mathbf k,0)\zeta(\mathbf p,\tau)\rangle=(2\pi)^3\delta^{(3)}(\mathbf k+\mathbf p)u_k(0)u_k^*(\tau).
$$

A differentiated vertex field instead supplies $u_k^{*\prime}(\tau)$. These conjugates are fixed by the [annihilation operators](../../../../../../../annihilation-operator.md) and [creation operators](../../../../../../../creation-operator.md) and cannot be dropped while retaining the same contour.

Convert the interaction time integral to [conformal time](../../../../../../../conformal-time.md). Since $dt=a\,d\tau$ and each cosmic-time derivative is $a^{-1}\partial_\tau$, the integrated cubic vertex is

$$
\int dt\,H_{\mathrm{int}}=-M_{\mathrm{Pl}}^2\epsilon^2\int d\tau\,a^2\int d^3x\,\zeta\zeta'^2.
$$

The [in-in formalism](../../../../../../../keldysh-formalism.md) supplies $-2i$ multiplying the expectation of the Hamiltonian, so its negative sign gives $+2i$ multiplying this vertex. At nonzero external momenta, the connected contractions join each of the three external fields to one vertex field. There are six bijections, not three. Choosing which external field meets the undifferentiated vertex gives three cyclic choices; swapping the two differentiated fields gives a further factor of two. This is the [Wick-pairing multiplicity for a zeta zeta-prime-squared vertex](../../../../../../../wick-pairing-multiplicity-for-a-zeta-zeta-prime-squared-vertex.md).

For example, before the internal momenta are integrated, one cyclic contribution includes

$$
\int\prod_{r=1}^3\frac{d^3p_r}{(2\pi)^3}\,(2\pi)^3\delta^{(3)}(\mathbf p_1+\mathbf p_2+\mathbf p_3)\prod_{r=1}^3[(2\pi)^3\delta^{(3)}(\mathbf k_r+\mathbf p_r)]\,u_{p_1}^*u_{p_2}^{*\prime}u_{p_3}^{*\prime}.
$$

The factors of $2\pi$ cancel to leave one overall $(2\pi)^3$ and the external momentum delta. Thus the properly normalized reduced expression is

$$
\boxed{\begin{aligned}
\langle\zeta_1\zeta_2\zeta_3\rangle_c&=(2\pi)^3\delta^{(3)}(\mathbf k_1+\mathbf k_2+\mathbf k_3)\\
&\quad\times\operatorname{Re}\left[4iM_{\mathrm{Pl}}^2\epsilon^2\prod_ru_{k_r}(0)\int_{-\infty(1-i\varepsilon)}^0d\tau\,a^2\sum_{\mathrm{cyc}}u_{k_1}^*u_{k_2}^{*\prime}u_{k_3}^{*\prime}\right].
\end{aligned}}
$$

The [vacuum prescription for inflationary in-in integrals](../../../../../../../vacuum-prescription-for-inflationary-in-in-integrals.md) damps the early-time oscillations and selects the [Bunch-Davies vacuum](../../../../../../../bunch-davies-vacuum.md). Internal self-contractions correspond to disconnected zero-momentum tadpole terms and are excluded from this connected three-point function.

The printed intermediate expression has unconjugated modes and only three literal cyclic terms with coefficient $-2i$. The conjugate form of the result above would use $-4i$, together with the conjugated contour. A literal $-2i$ with only three terms gives half the final printed answer. The six-contraction expression above is the consistent reduction of the supplied Hamiltonian and leads to that final answer.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 312](../../../../paper-312-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
