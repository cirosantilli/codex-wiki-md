<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Take $\eta^{\alpha\beta}=\operatorname{diag}(-1,1)$ with coordinate zero equal to $\tau$ and coordinate one to $\sigma$. In the supplied representation set

$$
C=\rho^0=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\qquad
\rho^1=\begin{pmatrix}0&1\\1&0\end{pmatrix}.
$$

They satisfy the [Clifford algebra](../../../../../clifford-algebra.md) $\{\rho^\alpha,\rho^\beta\}=2\eta^{\alpha\beta}\mathbf1$. For anticommuting spinor components and an ordinary matrix $B$, relabelling the two summed indices gives

$$
\chi^TB\psi=-\psi^TB^T\chi.
$$

Now $C^T=-C$, whereas $C\rho^0=-\mathbf1$ and $C\rho^1=\operatorname{diag}(-1,1)$ are symmetric. Therefore the [Majorana Grassmann bilinear interchange](../../../../../majorana-grassmann-bilinear-interchange.md) yields

$$
\boxed{\bar\psi^1\psi^2=\bar\psi^2\psi^1,
\qquad\bar\psi^1\rho^\alpha\psi^2=-\bar\psi^2\rho^\alpha\psi^1.}
$$

These signs require fermionic, Grassmann-odd fields; commuting spinors would have the opposite interchange signs.

In flat [conformal gauge](../../../../../conformal-gauge.md), suppress the common factor $(4\pi\alpha')^{-1}$ and write the combined density as $\mathcal L=-\partial_\alpha X\cdot\partial^\alpha X+\bar\psi\cdot\rho^\alpha\partial_\alpha\psi$. The [supersymmetry](../../../../../supersymmetry-split.md) variation including its odd parameter is an even derivation. From $(\rho^\alpha)^TC=-C\rho^\alpha$ we obtain

$$
\delta\bar\psi=-\bar\epsilon\rho^\beta\partial_\beta X.
$$

Also $(C\rho^\alpha\rho^\beta)^T=-C\rho^\beta\rho^\alpha$, so interchanging odd spinors gives $\bar\chi\rho^\alpha\rho^\beta\epsilon=\bar\epsilon\rho^\beta\rho^\alpha\chi$. The two density variations, with target contractions understood, are therefore

$$
\begin{aligned}
\delta\mathcal L_B&=2\bar\epsilon\,\partial_\beta X\cdot\partial^\beta\psi,\\
\delta\mathcal L_F&=-\bar\epsilon\rho^\beta\rho^\alpha\partial_\beta X\cdot\partial_\alpha\psi
+\bar\epsilon\,\psi\cdot\Box X.
\end{aligned}
$$

In the second term the symmetric second derivative annihilates the antisymmetric part of $\rho^\beta\rho^\alpha$. Using $2\eta^{\alpha\beta}-\rho^\beta\rho^\alpha=\rho^\alpha\rho^\beta$ now gives the exact off-shell identity

$$
\boxed{\delta\mathcal L=\partial_\alpha
\left(\bar\epsilon\rho^\alpha\rho^\beta\psi\cdot\partial_\beta X\right).}
$$

Thus the action is invariant when this boundary flux vanishes and the transformation preserves the field boundary conditions, for example with suitable falloff or compatible supersymmetric endpoint conditions. On a spatial circle, periodic fields admit the constant parameter; antiperiodic fermions with periodic bosons require the local superconformal treatment, since a nonzero constant parameter would make the boson variation antiperiodic. The constant parameter and ordinary derivatives describe rigid [supersymmetry](../../../../../supersymmetry-split.md) in flat gauge; a locally supersymmetric curved-worldsheet formulation includes the [worldsheet gravitino](../../../../../worldsheet-gravitino.md). The result is the [rigid worldsheet supersymmetry boundary term](../../../../../rigid-worldsheet-supersymmetry-boundary-term.md) without using field equations.

For the commutator on $X$, keep the order of the odd parameters:

$$
[\delta_1,\delta_2]X
=\left(\bar\epsilon_1\rho^\alpha\epsilon_2
-\bar\epsilon_2\rho^\alpha\epsilon_1\right)\partial_\alpha X
=\boxed{\ell^\alpha\partial_\alpha X},
\qquad\boxed{\ell^\alpha=2\bar\epsilon_1\rho^\alpha\epsilon_2.}
$$

For the fermion, the order is equally important. Moving $\epsilon_2$ through both odd factors in $(\bar\epsilon_1\partial_\alpha\psi)\epsilon_2$ incurs two minus signs. Consequently

$$
[\delta_1,\delta_2]\psi=\rho^\alpha M\partial_\alpha\psi,
\qquad M=\epsilon_1\bar\epsilon_2-\epsilon_2\bar\epsilon_1.
$$

To check the spinor matrix explicitly, set $\epsilon_1=(a,b)^T$, $\epsilon_2=(c,d)^T$, with all four components anticommuting and monomials ordered $a,b,c,d$. Then

$$
M=\begin{pmatrix}ad+bc&-2ac\\2bd&-ad-bc\end{pmatrix},
\quad V^0=\bar\epsilon_1\rho^0\epsilon_2=-ac-bd,
\quad V^1=\bar\epsilon_1\rho^1\epsilon_2=-ac+bd.
$$

Direct multiplication gives $\rho^\alpha M+M\rho^\alpha=2V^\alpha\mathbf1$. Hence

$$
[\delta_1,\delta_2]\psi
=2V^\alpha\partial_\alpha\psi-M(\rho^\alpha\partial_\alpha\psi).
$$

Variation of the fermion action gives the [Dirac equation](../../../../../dirac-equation.md) $\rho^\alpha\partial_\alpha\psi=0$. On this equation the second term vanishes, proving

$$
\boxed{[\delta_1,\delta_2]\psi=\ell^\alpha\partial_\alpha\psi,
\quad\ell^0=-2(ac+bd),\quad\ell^1=2(bd-ac).}
$$

This is [on-shell closure of rigid worldsheet supersymmetry](../../../../../on-shell-closure-of-rigid-worldsheet-supersymmetry.md); the action's invariance was off shell, but its fermionic transformation algebra closes in this field content only on shell.

The associated [superconformal current](../../../../../superconformal-current.md) is proportional to $\psi\cdot\partial X$, of [conformal weight](../../../../../conformal-weight.md) $3/2$. Its fermionic modes $G_r$ extend the stress-tensor generators to the [N=1 super-Virasoro algebra](../../../../../n-1-super-virasoro-algebra.md):

$$
[L_m,G_r]=\left(\frac m2-r\right)G_{m+r},\qquad
\{G_r,G_s\}=2L_{r+s}+\frac c3\left(r^2-\frac14\right)\delta_{r+s,0}.
$$

The modes are half-integral in the [Neveu–Schwarz sector](../../../../../neveu-schwarz-sector.md) and integral in the [Ramond sector](../../../../../ramond-sector.md). Their anticommutator giving a [Virasoro generator](../../../../../virasoro-generator.md) is the conformal-mode counterpart of the translation commutator just derived. Ten coordinate bosons and ten Majorana fermions give matter [central charge](../../../../../central-charge.md) $c=10+10/2=15$, canceled by the usual reparametrization and [superconformal ghosts](../../../../../superconformal-ghost.md) in the critical [RNS string](../../../../../spinning-string.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
