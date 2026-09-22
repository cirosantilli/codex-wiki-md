<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**First-class reduction.** A regular set of independent [constraints](../../../../../constraint-mechanics.md) is [first class](../../../../../first-class-constraint.md) when their [Poisson brackets](../../../../../poisson-bracket.md) vanish on the [constraint surface](../../../../../constraint-surface.md), equivalently locally $\{\varphi_i,\varphi_j\}=C_{ij}{}^k\varphi_k$. The coefficients can be functions on phase space. With the generator $G=\sum_i\xi^i\varphi_i$, an infinitesimal canonical gauge transformation is

$$
\boxed{\delta F=\{F,G\}.}
$$

Each independent first-class condition removes one phase-space dimension, and quotienting its independent gauge orbit removes another. Thus the regular physical phase space has

$$
\boxed{\dim\Gamma_{\mathrm{phys}}=2N-2n.}
$$

This [regular first-class phase-space reduction](../../../../../regular-first-class-phase-space-reduction.md) requires independent [constraints](../../../../../constraint-mechanics.md) and gauge directions. The count can fail at singular strata or for reducible [constraints](../../../../../constraint-mechanics.md); first-class closure alone does not guarantee independence. For a concrete counterexample to counting redundant equations, take two canonical pairs and $\varphi_1=p_1$, $\varphi_2=2p_1$. Both equations are first class, but there is only one independent condition and one gauge direction. The surviving pair $(q^2,p_2)$ has dimension two, whereas blindly substituting $N=n=2$ gives zero.

**Oscillator [symplectic form](../../../../../symplectic-form.md).** The center-of-mass pair $(x^m,p_m)$ describes translations and total momentum. The nonzero Fourier coefficients $\alpha_k^m$ describe the standing-wave modes compatible with free-end [Neumann boundary conditions](../../../../../neumann-boundary-condition.md); their reality condition is $\alpha_{-k}=\alpha_k^*$, and $\alpha_0^m=\sqrt{2\alpha'}p^m$ in the standard normalization. For $k>0$, regarding $\alpha_k^m$ as a complex coordinate makes its conjugate momentum $i\alpha_{-k,m}/k$. Equivalently write $\alpha_k=(q_k+is_k)/\sqrt2$. Up to a total derivative, its kinetic term is $-q_k\cdot\dot s_k/k$, a real canonical form. Inverting this [oscillator symplectic form of an open string](../../../../../oscillator-symplectic-form-of-an-open-string.md) gives

$$
\boxed{\{x^m,p_n\}=\delta^m{}_n,\qquad
\{\alpha_j^m,\alpha_k^n\}=-ij\eta^{mn}\delta_{j+k,0}.}
$$

The zero oscillator commutes with nonzero oscillators but is not independent of $p$: $\{x^m,\alpha_0^n\}=\sqrt{2\alpha'}\eta^{mn}$. Brackets between the center pair and independent nonzero oscillators vanish.

The quadratic [constraints](../../../../../constraint-mechanics.md) obey

$$
\{\alpha_k^m,L_n\}=-ik\alpha_{k+n}^m.
$$

For example, the two terms in the bracket with $L_n=\tfrac12\sum_j\alpha_j\cdot\alpha_{n-j}$ give equal contributions after relabelling $j$. Applying this identity to both factors of $L_m$ gives

$$
\boxed{\{L_m,L_n\}=-i(m-n)L_{m+n}.}
$$

This [classical Virasoro constraint algebra](../../../../../classical-virasoro-constraint-algebra.md) has no central term and closes on the [constraints](../../../../../constraint-mechanics.md), hence is first class. For $G=\sum_n\xi_{-n}L_n$, the oscillator gauge transformation is

$$
\boxed{\delta\alpha_k^m=-ik\sum_n\xi_{-n}\alpha_{k+n}^m.}
$$

Reality is respected when $\xi_{-n}=\xi_n^*$.

**Light-cone reduction and mass.** Choose [light-cone coordinates](../../../../../light-cone-coordinates.md) $X^\pm=(X^0\pm X^{D-1})/\sqrt2$; a vector square is $-2\alpha^+\alpha^-+\boldsymbol\alpha^2$, with $D-2$ transverse components. On the proposed gauge slice $\alpha_{k\ne0}^+=0$, the variation becomes

$$
\delta\alpha_k^+=-ik\xi_k\alpha_0^+.
$$

For $\alpha_0^+\ne0$, every nonzero-mode gauge parameter has an invertible coefficient, so the conditions locally fix the corresponding gauge freedom. Globally this is the usual patch in which $X^+$ is an admissible [worldsheet](../../../../../worldsheet.md) clock; it is not a claim about strings for which that coordinate has turning points. The zero-mode reparameterization is left over.

On that slice the nonzero [Virasoro constraints](../../../../../virasoro-constraint.md) are linear in the longitudinal oscillators:

$$
\boxed{\alpha_k^-=\frac1{2\alpha_0^+}
\sum_j\boldsymbol\alpha_j\cdot\boldsymbol\alpha_{k-j},\qquad k\ne0.}
$$

No nonzero longitudinal oscillator remains independent. The residual action is

$$
S_{\mathrm{red}}=\int dt\left[
\dot x^mp_m+\sum_{k>0}\frac{i}{k}\boldsymbol\alpha_{-k}\cdot\dot{\boldsymbol\alpha}_k
-\lambda_0\left(\alpha'p^2+\sum_{k>0}\boldsymbol\alpha_{-k}\cdot\boldsymbol\alpha_k\right)\right].
$$

This [residual mass-shell action in light-cone string gauge](../../../../../residual-mass-shell-action-in-light-cone-string-gauge.md) displays the remaining zero-mode [constraint](../../../../../constraint-mechanics.md). At the quantum level [normal ordering](../../../../../normal-ordering.md) replaces its oscillator term by $N-a$. One can further set $x^+$ equal to time and solve for the [light-cone Hamiltonian](../../../../../light-cone-hamiltonian.md) $p^-=[\boldsymbol p^2+(N-a)/\alpha']/(2p^+)$.

Canonical quantization gives the transverse relations

$$
\boxed{[\alpha_j^I,\alpha_k^J]=j\delta^{IJ}\delta_{j+k,0}.}
$$

Here $\hbar=1$, $\alpha_{k>0}$ annihilate the [oscillator vacuum](../../../../../oscillator-vacuum.md), and $\alpha_{-k}$ create excitations. Define $a_k^I=\alpha_k^I/\sqrt k$ for $k>0$. The [string level operator](../../../../../string-level-operator.md) is

$$
N=\sum_{k>0,I}\alpha_{-k}^I\alpha_k^I
=\sum_{k>0,I}k\,a_k^{I\dagger}a_k^I.
$$

Thus it counts oscillator number weighted by mode number, and has nonnegative integer eigenvalues. The residual [mass-shell condition](../../../../../string-mass-shell-condition.md) gives

$$
\boxed{\mathcal M^2=-p^2=\frac{N-a}{\alpha'},\qquad
\alpha'=\frac1{2\pi T}.}
$$

The constant $a$ is the [normal-ordering constant of a string](../../../../../normal-ordering-constant-of-a-string.md), or intercept, not an extra classical tension. In the usual Lorentz-invariant critical bosonic string, level one carries the $D-2$ transverse polarizations of a massless vector. A massive vector would need $D-1$ polarizations; the longitudinal one is not present. Lorentz consistency therefore requires that this vector level be massless, giving **$a=1$**. Equivalently the regularized transverse zero-point value $a=(D-2)/24$ gives $D=26$. This [critical-vector assumption in the string intercept argument](../../../../../critical-vector-assumption-in-the-string-intercept-argument.md) concerns the usual critical quantum theory. In $D=3$ the lone transverse level-one polarization transforms trivially under the transverse rotation group; a massive scalar interpretation is not excluded by counting. Thus the stated masslessness conclusion is not a consequence of polarization counting for arbitrary $D$. An arbitrary intercept in a transverse oscillator model also need not define the usual covariant critical theory.

**The full self-dual massless spectrum.** In the closed-string sector, $N$ and $\widetilde N$ are the independent nonnegative integer oscillator levels of the two chiral sectors. The integer $n$ quantizes center momentum around the circle, $p_{\mathrm{circle}}=n/R$, and $w$ counts how many times the string winds it. At the [self-dual circle](../../../../../self-dual-circle-compactification.md) $R=\sqrt{\alpha'}$, zero mass requires

$$
2(N+\widetilde N-2)+n^2+w^2=0,
\qquad N-\widetilde N=nw.
$$

Both levels are nonnegative, so their sum is at most two. Exhausting these possibilities gives the [massless spectrum at the bosonic self-dual circle](../../../../../massless-spectrum-at-the-bosonic-self-dual-circle.md):

- $N=\widetilde N=1$, $(n,w)=(0,0)$: all states $\alpha_{-1}^I\widetilde\alpha_{-1}^J|0;n=0,w=0\rangle$, with arbitrary transverse polarizations.
- $N=1,\widetilde N=0$, $(n,w)=(1,1)$ or $(-1,-1)$: one left-sector level-one oscillator with any transverse polarization.
- $N=0,\widetilde N=1$, $(n,w)=(1,-1)$ or $(-1,1)$: one right-sector level-one oscillator with any transverse polarization.
- $N=\widetilde N=0$, $(n,w)=(2,0),(-2,0),(0,2),(0,-2)$: four oscillator ground states made massless by their momentum or winding energy.

The last family is easy to miss because the uncompactified ground state is a [tachyon](../../../../../tachyon.md); its positive compact energy cancels that negative contribution at these charges. There are no other possibilities: at level sum one, $n^2+w^2=2$ forces both charges to be $\pm1$; at sum zero, $n^2+w^2=4$ gives exactly the four listed pairs. With $d=D-2$ transverse oscillators the number of independent massless polarizations is $d^2+4d+4=D^2$, hence **676 in the critical $D=26$ bosonic theory**. The circle oscillator is included among the $d$ components; it should not be discarded when interpreting the lower-dimensional scalar states.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
