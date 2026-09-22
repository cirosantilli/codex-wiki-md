<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use $\partial_\pm=(\partial_\tau\pm\partial_\sigma)/2$ and keep each constant odd supersymmetry parameter on the left. The transformation of a fermion may be written $\delta\psi_1^\mu=\epsilon_1\partial_+X^\mu$ or $\partial_+X^\mu\epsilon_1$, since the bosonic derivative commutes with the parameter. The variation $\delta$ itself is even, so it obeys the ordinary product rule; the signs below arise when moving an odd parameter past an odd field.

First consider the $\epsilon_1$ transformation. Suppress target indices and put $\mathcal L=2X_+\cdot X_-+i\psi_1\cdot\partial_-\psi_1+i\psi_2\cdot\partial_+\psi_2$. Its bosonic part varies as

$$
\delta_1\mathcal L_X=-i\epsilon_1\big(\partial_+\psi_1\cdot X_-+X_+\cdot\partial_-\psi_1\big).
$$

For the first fermion, moving $\epsilon_1$ to the left gives

$$
\begin{aligned}
\delta_1\mathcal L_{\psi_1}
&=i\big((\epsilon_1X_+)\cdot\partial_-\psi_1+\psi_1\cdot\partial_-(\epsilon_1X_+)\big)\\
&=i\epsilon_1\big(X_+\cdot\partial_-\psi_1-\psi_1\cdot\partial_-X_+\big).
\end{aligned}
$$

The second fermion does not vary under $\epsilon_1$. Since $\partial_-X_+=\partial_+X_-$, these terms combine to $\delta_1\mathcal L=-i\epsilon_1\partial_+(\psi_1\cdot X_-)$. The other parameter gives the same cancellation with $+\leftrightarrow-$ and $1\leftrightarrow2$. Therefore

$$
\boxed{\delta I=-\frac i\pi\int d\sigma d\tau\,\left[\epsilon_1\partial_+(\psi_1\cdot\partial_-X)+\epsilon_2\partial_-(\psi_2\cdot\partial_+X)\right].}
$$

This proves [worldsheet supersymmetry](../../../../../worldsheet-supersymmetry.md) invariance up to the [rigid worldsheet supersymmetry boundary term](../../../../../rigid-worldsheet-supersymmetry-boundary-term.md), without using field equations.

For an open string, the boundary term is part of the invariance statement. For example, a Neumann endpoint has $\partial_+X=\partial_-X$ and compatible fermion gluing $\psi_1=\kappa\psi_2$, $\kappa=\pm1$. The spatial boundary flux vanishes when $\epsilon_2=\kappa\epsilon_1$. Both endpoints must admit the same preserved parameter. Opposite gluing signs, giving the [Neveu–Schwarz sector](../../../../../neveu-schwarz-sector.md), do not preserve a nonzero constant parameter at both ends. Thus the local bulk identity and the existence of a global rigid charge on a particular open-string sector are distinct. The local superconformal symmetry remains the basis of the string constraints; this is consistent with the [spin-structure obstruction to constant worldsheet supersymmetry](../../../../../spin-structure-obstruction-to-constant-worldsheet-supersymmetry.md).

Now write $A_\pm^\mu=\partial_\pm X^\mu$ and $J_+^1=\psi_1\cdot A_+$, $J_-^2=\psi_2\cdot A_-$. The other two components vanish. The action implies $\partial_-\psi_1=0$, $\partial_+\psi_2=0$ and $\partial_+\partial_-X=0$, so these [supercurrents](../../../../../supercurrent.md) are chiral and conserved locally. At equal time, the given [canonical commutation relations](../../../../../canonical-commutation-relation.md) imply

$$
[A_\pm^\mu(\sigma),X^\nu(\sigma')]= -\frac{i\pi}{2}\eta^{\mu\nu}\delta(\sigma-\sigma').
$$

With $q_\epsilon=\pi^{-1}\int d\sigma(\epsilon_1\psi_1\cdot A_++\epsilon_2\psi_2\cdot A_-)$, contraction with this commutator gives

$$
\boxed{[q_\epsilon,X^\mu]= -\frac i2\epsilon_1\psi_1^\mu-\frac i2\epsilon_2\psi_2^\mu.}
$$

The parameter-weighted charge is even. Since the parameters anticommute with the fermions,

$$
[\epsilon_i\psi_i^\nu A_{\pm\nu},\psi_j^\mu]
=\epsilon_i\{\psi_i^\nu,\psi_j^\mu\}A_{\pm\nu}.
$$

Using the PDF's normalization $\{\psi_i^\mu(\sigma),\psi_j^\nu(\sigma')\}=\pi\eta^{\mu\nu}\delta_{ij}\delta(\sigma-\sigma')$ yields

$$
\boxed{[q_\epsilon,\psi_1^\mu]=\epsilon_1\partial_+X^\mu,\qquad [q_\epsilon,\psi_2^\mu]=\epsilon_2\partial_-X^\mu.}
$$

Thus the charge generates all the specified [supersymmetry transformations](../../../../../supersymmetry-transformation.md). Dropping the factor $\pi$ in the fermion anticommutator, as happens in the converted TeX, would fail this check. The original PDF has the correct factor.

To calculate the supercurrent bracket, put $A=\partial_+X$ and $J=\psi_1\cdot A$. The equal-time bosonic relations give

$$
\begin{aligned}
[A^\mu(\sigma),A^\nu(\sigma')]
&=\frac14\left([\dot X^\mu(\sigma),X'^{\nu}(\sigma')]+[X'^{\mu}(\sigma),\dot X^\nu(\sigma')]\right)\\
&=\frac{i\pi}{2}\eta^{\mu\nu}\partial_\sigma\delta(\sigma-\sigma').
\end{aligned}
$$

Bosonic and fermionic fields commute. Expanding the two current products, commuting the bosonic factors once and using the fermion anticommutator gives the noncentral part

$$
\{J(\sigma),J(\sigma')\}_{\rm nc}
=\pi\delta(\sigma-\sigma')A(\sigma')\cdot A(\sigma)
+\frac{i\pi}{2}\partial_\sigma\delta(\sigma-\sigma')\,\psi_1(\sigma)\cdot\psi_1(\sigma').
$$

For an ordinary smooth bilocal coefficient, the [distributional derivative](../../../../../distributional-derivative.md) identity is

$$
f(\sigma,\sigma')\partial_\sigma\delta(\sigma-\sigma')
=f(\sigma,\sigma)\partial_\sigma\delta(\sigma-\sigma')
+\left.\partial_{\sigma'}f(\sigma,\sigma')\right|_{\sigma'=\sigma}\delta(\sigma-\sigma').
$$

For the fermion bilinear, its coincident classical value, or its coincident normal-ordered value, is zero by antisymmetry against the symmetric target metric. The second term is $\psi_1\cdot\partial_\sigma\psi_1$. Since $\partial_-\psi_1=0$, we have $\partial_\sigma\psi_1=\partial_+\psi_1$. It follows that the noncentral current bracket is

$$
\boxed{\{J_+^1(\sigma),J_+^1(\sigma')\}_{\rm nc}=\pi\delta(\sigma-\sigma')\theta_{++}(\sigma),\qquad
\theta_{++}=(\partial_+X)^2+\frac i2\psi_1\cdot\partial_+\psi_1.}
$$

This is the [canonical supercurrent bracket of free RNS matter](../../../../../canonical-supercurrent-bracket-of-free-rns-matter.md). The other chirality similarly gives $\theta_{--}=(\partial_-X)^2+(i/2)\psi_2\cdot\partial_-\psi_2$ and $\theta_{+-}=0$ on shell.

The printed current identity is the classical, or noncentral, part of the algebra. Fully quantized coincident products require [normal ordering](../../../../../normal-ordering.md); the matter algebra then also has a central contact term proportional to $\delta''$ in the current anticommutator. The 10 bosons and 10 real fermions contribute matter [central charge](../../../../../central-charge.md) $c=10+10/2=15$. The central term cannot be discarded in a literal quantum operator identity, although it is irrelevant to identifying the local noncentral stress tensor above.

The other brackets close on these same currents. The stress-tensor commutator contains $\theta\delta'$ and $\theta'\delta$ and, quantum mechanically, a central $\delta'''$ term. The stress-tensor–supercurrent commutator contains $J\delta'$ and $J'\delta$, expressing the [conformal weight](../../../../../conformal-weight.md) $3/2$ of $J$. The supercurrent anticommutator contains $\theta\delta$ and its central $\delta''$ term. In a conventional normalization of Fourier modes these form the [N=1 super-Virasoro algebra](../../../../../n-1-super-virasoro-algebra.md):

$$
\begin{aligned}
[L_m,L_n]&=(m-n)L_{m+n}+C_{mn}\mathbf1,\\
[L_m,G_r]&=\left(\frac m2-r\right)G_{m+r},\\
\{G_r,G_s\}&=2L_{r+s}+D_{rs}\mathbf1.
\end{aligned}
$$

Here $C_{mn}$ and $D_{rs}$ are central terms supported at zero total mode number; their detailed coefficients are not needed for this request. The indices $r$ are half-integers in the [Neveu–Schwarz sector](../../../../../neveu-schwarz-sector.md) and integers in the [Ramond sector](../../../../../ramond-sector.md). Opposite chiralities commute or anticommute as appropriate.

For the closed [RNS string](../../../../../spinning-string.md), impose a copy of the constraints in each chirality. In the [Neveu–Schwarz sector](../../../../../neveu-schwarz-sector.md), the physical conditions are

$$
L_{n>0}|\Psi\rangle=0,\qquad G_{r>0}|\Psi\rangle=0,\qquad (L_0-a_{\rm NS})|\Psi\rangle=0,\qquad a_{\rm NS}=\frac12.
$$

In the [Ramond sector](../../../../../ramond-sector.md), use vacuum-normal-ordered generators with zero Ramond intercept. Then

$$
L_{n>0}|\Psi\rangle=0,\qquad G_{n>0}|\Psi\rangle=0,\qquad G_0|\Psi\rangle=0,\qquad L_0|\Psi\rangle=0.
$$

The Ramond zero-mode equation is essential: its square gives the mass-shell condition in this convention, $G_0^2=L_0$, and on the oscillator ground sector it is the spacetime Dirac constraint. In a convention whose unshifted plane generator has $G_0^2=L_0-c/24$, the zero-mode equation instead sets that shifted combination to zero; these are the same condition, not competing intercepts.

For either choice, the corresponding tilded constraints hold on the other side. Both chiral mass-shell conditions and [closed-string level matching](../../../../../closed-string-level-matching.md) are required:

$$
\boxed{N_L-a_L=N_R-a_R,\qquad M^2=\frac4{\alpha'}(N_L-a_L),\qquad a_{\rm NS}=\frac12,\quad a_{\rm R}=0.}
$$

The state sectors are NS–NS, NS–R, R–NS and R–R. Quotienting physical null states removes unphysical longitudinal polarizations; equivalently, use the appropriate [BRST cohomology](../../../../../brst-cohomology.md) including the superconformal ghosts. A consistent superstring also specifies the [GSO projection](../../../../../gso-projection.md). It is an additional sector selection, not a replacement for these local super-Virasoro constraints. **Physical states satisfy both chiral positive-mode and zero-mode constraints, level matching, and the null-state quotient; Ramond states additionally obey the fermionic zero-mode constraint.**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 53](../../paper-53-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
