<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Spinning-particle mechanics.** Keep the mostly-plus metric and place the odd multiplier $\chi$ to the left. Varying the original PDF's dotted-fermion kinetic term gives

$$
\boxed{\dot p_m=0,\qquad \dot x^m=e p^m+i\chi\zeta^m,
\qquad\dot\zeta^m=-\chi p^m,\qquad p^2=0,\qquad p\cdot\zeta=0.}
$$

The last two equations are multiplier [constraints](../../../../../constraint-mechanics.md). In deriving the [fermion](../../../../../fermion.md) equation, the variation of $i\zeta\cdot\dot\zeta/2$ is $i\delta\zeta\cdot\dot\zeta$ after integration by parts; moving $\delta\zeta$ past $\chi$ supplies the sign in the interaction variation. The TeX conversion omits the dot, which would erase the fermionic symplectic structure; the PDF fixes it.

Under an infinitesimal Lorentz rotation the target vectors $x,p,\zeta$ transform together. The scalar contractions in the action are invariant. Its antisymmetric [Noether charge](../../../../../noether-charge.md) is

$$
\boxed{J^{mn}=x^mp^n-x^np^m-i\zeta^m\zeta^n,
\qquad S^{mn}=-i\zeta^m\zeta^n.}
$$

The spin bilinear is antisymmetric because the [Grassmann variables](../../../../../grassmann-variable.md) anticommute. Direct differentiation makes conservation particularly transparent:

$$
\frac d{dt}(x^mp^n-x^np^m)
=i\chi(\zeta^mp^n-\zeta^np^m),
$$

while the [fermion](../../../../../fermion.md) equation gives

$$
\frac d{dt}S^{mn}=-i\chi(\zeta^mp^n-\zeta^np^m).
$$

They cancel, so $\dot J^{mn}=0$. The same charge generates [Lorentz transformations](../../../../../lorentz-transformation.md) through the canonical and fermionic [Dirac brackets](../../../../../dirac-bracket.md), up to the convention for the sign of the antisymmetric transformation parameter.

The [pseudoclassical spinning particle](../../../../../pseudoclassical-spinning-particle.md) uses odd classical variables rather than assigning an ordinary commuting spatial vector to spin. Eliminating the fermionic momentum [constraints](../../../../../constraint-mechanics.md) gives

$$
\boxed{\{\zeta^m,\zeta^n\}_{D}=-i\eta^{mn}.}
$$

These are symmetric [graded Poisson brackets](../../../../../graded-poisson-bracket.md). The even bilinears $S^{mn}$ have the [Lorentz transformation](../../../../../lorentz-transformation.md) law of an internal angular-momentum tensor. This is [spin from Grassmann bilinears](../../../../../spin-from-grassmann-bilinears.md).

Quantization replaces the bracket by an anticommutator,

$$
\{\widehat\zeta^m,\widehat\zeta^n\}_+=\eta^{mn},
\qquad\widehat\zeta^m=\frac1{\sqrt2}\gamma^m,
\quad\{\gamma^m,\gamma^n\}_+=2\eta^{mn}.
$$

The [Clifford algebra](../../../../../clifford-algebra.md) is represented on spinors. The [constraint](../../../../../constraint-mechanics.md) $p\cdot\zeta=0$ then becomes

$$
\boxed{\gamma^m\partial_m\Psi(x)=0,}
$$

the [massless Dirac equation](../../../../../massless-dirac-equation.md). Its square gives the massless wave equation, matching $p^2=0$. The quantized spin generator is $-i[\gamma^m,\gamma^n]/4$. This [spinning-particle Dirac quantization](../../../../../spinning-particle-dirac-quantization.md) explains why the wavefunction carries a spinor index even though the original $x$ variables are vector coordinates.

**The NS phase-space action.** A Fourier action compatible with the displayed [constraints](../../../../../constraint-mechanics.md) is

$$
\boxed{S_{\mathrm{NS}}=\int dt\left[
\dot x\cdot p+\sum_{k>0}\frac{i}{k}\alpha_{-k}\cdot\dot\alpha_k
+i\sum_{r>0}b_{-r}\cdot\dot b_r
-\sum_{n\in\mathbb Z}\lambda_{-n}L_n
-i\sum_{r\in\mathbb Z+1/2}\chi_{-r}G_r\right].}
$$

The $\chi_r$ are odd multipliers; an overall phase can instead be absorbed in their definition. The $b_r$ here are fermionic matter modes, not the $b$ antighost of Question3. This [Neveu–Schwarz Fourier phase-space action](../../../../../neveu-schwarz-fourier-phase-space-action.md) gives the bosonic oscillator [symplectic form](../../../../../symplectic-form.md) and $\{b_r^m,b_s^n\}_{\mathrm{PB}}=-i\eta^{mn}\delta_{r+s,0}$.

For an open string, the two [worldsheet](../../../../../worldsheet.md) [fermion](../../../../../fermion.md) chiralities are related at each endpoint. Opposite relative signs at the two ends produce, after doubling the interval, $\psi(\sigma+2\pi)=-\psi(\sigma)$. The [Neveu–Schwarz sector](../../../../../neveu-schwarz-sector.md) therefore has half-integer Fourier frequencies $r\in\mathbb Z+1/2$, with no matter-fermion zero mode. Equal endpoint signs give the periodic Ramond sector instead. The bosonic zero-mode normalization is again $\alpha_0=\sqrt{2\alpha'}p$.

In [old covariant string quantization](../../../../../old-covariant-string-quantization.md), all target components are retained and obey

$$
\boxed{[\alpha_k^m,\alpha_l^n]=k\eta^{mn}\delta_{k+l,0},
\qquad\{b_r^m,b_s^n\}_+=\eta^{mn}\delta_{r+s,0}.}
$$

Other oscillator brackets vanish. The momentum-labelled [oscillator vacuum](../../../../../oscillator-vacuum.md) satisfies $\alpha_{k>0}|0;p\rangle=b_{r>0}|0;p\rangle=0$, $\widehat p_m|0;p\rangle=p_m|0;p\rangle$, and $\alpha_0=\sqrt{2\alpha'}p$; take its matter norm positive. The zero-point convention stated in the question gives

$$
L_0=\alpha'p^2+N_{\mathrm{NS}},\qquad
N_{\mathrm{NS}}=\sum_{k>0}\alpha_{-k}\cdot\alpha_k
+\sum_{r>0}r\,b_{-r}\cdot b_r.
$$

A physical oscillator ground state has $\alpha'p^2=a$, so

$$
\boxed{M_0^2=-\frac a{\alpha'}.}
$$

It is a scalar, not a spinor, since the NS sector has no Clifford zero modes. It is a [tachyon](../../../../../tachyon.md) if $a>0$, massless if $a=0$, and massive if $a<0$. In the usual limiting $a=1/2$ theory it is the unprojected NS [tachyon](../../../../../tachyon.md), removed by the standard [GSO projection](../../../../../gso-projection.md). Calling it tachyonic before specifying the sign of $a$ would be too strong.

**The half-level vector and its norm.** Let $|A;p\rangle=A_m(p)b_{-1/2}^m|0;p\rangle$. The level is $N_{\mathrm{NS}}=1/2$. Its $L_0$ condition and the only potentially nonzero positive supercurrent condition give

$$
\boxed{\alpha'p^2+\frac12-a=0,\qquad p\cdot A=0.}
$$

Indeed $\{G_{1/2},b_{-1/2}^m\}=\alpha_0^m$ implies $G_{1/2}|A;p\rangle=\sqrt{2\alpha'}p\cdot A|0;p\rangle$. Higher positive $G_r$ annihilate the state. Likewise $[L_n,b_{-1/2}^m]=(1/2-n/2)b_{n-1/2}^m$ is either zero or an annihilator, so all $L_{n>0}$ conditions hold. This is the [half-level Neveu–Schwarz vector state](../../../../../half-level-neveu-schwarz-vector-state.md).

Its matter norm is proportional to $A^*\cdot A$. For a real, nonzero on-shell momentum in ordinary $D\ge2$ Minkowski space, three cases exhaust the possibilities:

- If $a<1/2$, then $p$ is timelike and its orthogonal complement is Euclidean. In its rest frame $p\cdot A=0$ sets $A^0=0$, so every nonzero physical polarization has positive norm.
- If $a=1/2$, then $p$ is null. Choose $p=E(1,0,\ldots,0,1)$, $E\ne0$. Transversality sets $A^{D-1}=A^0$, leaving $A^*\cdot A=\sum_{I=1}^{D-2}|A^I|^2\ge0$. Polarizations proportional to $p$ are null.
- If $a>1/2$, then $p$ is spacelike. A frame with $p=(0,k,0,\ldots)$ allows $A=(1,0,\ldots)$, which satisfies $p\cdot A=0$ but has norm $-1$. It is an explicit negative-norm physical polarization at this level.

Thus, with the usual nonzero particle-momentum hypothesis,

$$
\boxed{\text{all physical half-level vector polarizations have nonnegative norm}
\quad\Longleftrightarrow\quad a\le\frac12.}
$$

This is a level-specific result, not a proof of the full NS no-ghost theorem in arbitrary dimension.

At the limiting intercept the vector becomes massless, and the longitudinal polarization is a null state. It is generated by $G_{-1/2}|0;p\rangle=\sqrt{2\alpha'}p\cdot b_{-1/2}|0;p\rangle$. Factoring out that null direction identifies $A\sim A+\kappa p$ and leaves $D-2$ positive physical polarizations of a gauge vector. In the consistent critical NS string one additionally has $D=10$; the half-level positivity argument alone does not derive that dimension.

There is a genuine zero-momentum exception if the printed word “all” is read literally. At $a=1/2$ and $p=0$, the polarization $A=(1,0,\ldots)$ obeys every displayed positive-mode [constraint](../../../../../constraint-mechanics.md) and the mass shell, but has norm $-1$. Transversality is vacuous, and $A\sim A+\kappa p$ removes nothing. This [nonzero-momentum condition in the massless vector norm test](../../../../../nonzero-momentum-condition-in-the-massless-vector-norm-test.md) is therefore necessary for the intended endpoint assertion. Including zero momentum changes the unrestricted elementary test to strict $a<1/2$; ordinary propagating massless particle states use nonzero null momentum.

Finally, an [oscillator vacuum](../../../../../oscillator-vacuum.md) used to build the excited state is labelled by that state's momentum. It need not separately satisfy the scalar-ground-state mass shell: imposing both $\alpha'p^2=a$ and $\alpha'p^2=a-1/2$ at the same momentum would incorrectly exclude all such excitations.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
