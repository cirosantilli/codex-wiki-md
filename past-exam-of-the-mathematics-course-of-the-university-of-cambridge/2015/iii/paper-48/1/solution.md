<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the minimal four-dimensional [Super-Poincaré algebra](../../../../../super-poincare-algebra.md), with $\{Q_\alpha,Q_\beta\}=0$, $\{Q_\alpha,\bar Q_{\dot\beta}\}=2\sigma^\nu_{\alpha\dot\beta}P_\nu$ and commuting translations. [Lorentz covariance](../../../../../lorentz-covariance.md) and closure on the existing [supercharges](../../../../../supersymmetry-generator.md) permit only

$$
[P^\mu,Q_\alpha]=A(\sigma^\mu)_{\alpha\dot\gamma}\bar Q^{\dot\gamma}.
$$

The [graded Jacobi identity](../../../../../graded-jacobi-identity.md) for $P^\mu,Q_\alpha,Q_\beta$ therefore gives

$$
0=\{[P^\mu,Q_\alpha],Q_\beta\}+\{Q_\alpha,[P^\mu,Q_\beta]\}
=2A\left(\sigma^\mu_{\alpha\dot\gamma}\epsilon^{\dot\gamma\dot\delta}\sigma^\nu_{\beta\dot\delta}+\sigma^\mu_{\beta\dot\gamma}\epsilon^{\dot\gamma\dot\delta}\sigma^\nu_{\alpha\dot\delta}\right)P_\nu.
$$

For example, with $\sigma^0=I$, $\mu=0$ and $\alpha=\beta=1$, the coefficient is a nonzero multiple of $A(P_1-iP_2)$. Independence of the translation generators forces $A=0$. Its adjoint gives the barred result. Thus **every supercharge commutes with four-momentum**:

$$
\boxed{[Q_\alpha,P^\mu]=0.}
$$

Consequently $[Q_\alpha,P^2]=0$. If $|u\rangle$ has a particular [mass-shell condition](../../../../../string-mass-shell-condition.md), the nonzero state $Q_\alpha|u\rangle$ has the same one. This gives [supersymmetric mass degeneracy](../../../../../supersymmetric-mass-degeneracy.md) within an unbroken physical [supermultiplet](../../../../../supermultiplet.md). The qualification matters: after spontaneous [supersymmetry breaking](../../../../../supersymmetry-breaking.md), the chosen vacuum is not annihilated by the [supercharges](../../../../../supersymmetry-generator.md), and its one-particle excitations need not constitute degenerate [supermultiplets](../../../../../supermultiplet.md).

For the [O'Raifeartaigh model](../../../../../o-raifeartaigh-model.md), write $X=\phi_1$, $Y=\phi_2$, $Z=\phi_3$. Field phases allow $g,M,m$ to be positive. The canonical [Kähler potential](../../../../../kahler-potential.md) and elimination of the [auxiliary fields](../../../../../auxiliary-field.md) give the [F-term scalar potential](../../../../../f-term-scalar-potential.md)

$$
V=g^2|Z^2-m^2|^2+M^2|Z|^2+|2gXZ+MY|^2.
$$

A [supersymmetric vacuum](../../../../../supersymmetric-vacuum.md) would require $W_Y=MZ=0$, hence $Z=0$, while $W_X=g(Z^2-m^2)=-gm^2$ could not vanish. Thus [F-flatness](../../../../../f-flatness.md) is impossible. More precisely, with $Z=u+iv$,

$$
V=g^2m^4+(M^2-2g^2m^2)u^2+(M^2+2g^2m^2)v^2+g^2(u^2+v^2)^2+|2gXZ+MY|^2.
$$

The stated strict inequality makes every nonconstant term nonnegative. **The entire classical vacuum family is**

$$
\boxed{Z=Y=0,\qquad X=x\text{ arbitrary},\qquad V_0=g^2m^4>0.}
$$

Here $F_X=-\overline{W_X}=gm^2$, while $F_Y=F_Z=0$. The [Weyl spinor](../../../../../weyl-spinor.md) $\psi_X$ is the massless [goldstino](../../../../../goldstino.md), and the [complex scalar field](../../../../../complex-scalar-field.md) $X$ is a [pseudomodulus](../../../../../pseudomodulus.md) with two zero tree-level squared masses. The hierarchy $M\gg m$ separates the massive fields from the breaking scale, but it does not itself select $x=0$ along this flat direction.

At the representative vacuum $x=0$, the [chiral-superfield fermion mass matrix](../../../../../chiral-superfield-fermion-mass-matrix.md) is

$$
m_F=\begin{pmatrix}0&0&0\\0&0&M\\0&M&0\end{pmatrix}.
$$

Its physical masses are its [singular values](../../../../../singular-value.md): $0,M,M$. The two massive [Weyl spinors](../../../../../weyl-spinor.md) can be combined into one massive [Dirac spinor](../../../../../dirac-spinor.md). For $Y=(y_R+iy_I)/\sqrt2$, $Z=(z_R+iz_I)/\sqrt2$, the real scalar squared masses are

$$
\boxed{m_{X_R}^2=m_{X_I}^2=0,\quad m_{y_R}^2=m_{y_I}^2=M^2,\quad m_{z_R}^2=M^2-2g^2m^2,\quad m_{z_I}^2=M^2+2g^2m^2.}
$$

In particular, there is no [tachyon](../../../../../tachyon.md) under the stated inequality. The splitting of the $Z$ masses displays [supersymmetry breaking](../../../../../supersymmetry-breaking.md) directly.

For completeness, the mass spectrum can be given throughout the classical vacuum family, rather than silently fixing the [pseudomodulus](../../../../../pseudomodulus.md). A phase rotation makes $x$ real and nonnegative without changing physical masses. The massive fermion squared masses are

$$
f_\pm=M^2+2g^2|x|^2\pm2g|x|\sqrt{M^2+g^2|x|^2}.
$$

The real and imaginary scalar sectors have two-by-two [scalar squared-mass matrices](../../../../../scalar-mass-matrix.md)

$$
B_\epsilon=\begin{pmatrix}M^2&2gM|x|\\2gM|x|&M^2+4g^2|x|^2+2\epsilon g^2m^2\end{pmatrix},\qquad\epsilon=-1,+1,
$$

whose [eigenvalues](../../../../../eigenvalue.md) are

$$
b_{\epsilon,\pm}=M^2+2g^2|x|^2+\epsilon g^2m^2\pm\sqrt{(2g^2|x|^2+\epsilon g^2m^2)^2+4g^2M^2|x|^2}.
$$

Both [determinants](../../../../../determinant.md) are $M^2(M^2+2\epsilon g^2m^2)>0$ and their traces are positive, so stability holds at every finite $x$. Quantum corrections can lift a [pseudomodulus](../../../../../pseudomodulus.md); these formulas describe the classical, tree-level spectrum requested here.

Define the physical mass [supertrace](../../../../../supertrace.md) by

$$
\operatorname{STr}\mathcal M^2=\sum_s(-1)^{2s}(2s+1)\operatorname{tr}\mathcal M_s^2.
$$

Each real scalar contributes once and each [Weyl spinor](../../../../../weyl-spinor.md) twice with a minus sign. At $x=0$ this gives $4M^2-2(2M^2)=0$. At general $x$, $\sum_{\epsilon,\pm}b_{\epsilon,\pm}=4M^2+8g^2|x|^2=2(f_++f_-)$. Hence **the tree-level mass supertrace vanishes despite broken supersymmetry**:

$$
\boxed{\operatorname{STr}\mathcal M^2=0.}
$$

This is the [tree-level supertrace mass sum rule](../../../../../tree-level-supertrace-mass-sum-rule.md), not a claim that the individual masses are equal.

For direct breaking in the [Minimal supersymmetric Standard Model](../../../../../minimal-supersymmetric-standard-model.md), the difficulty is both field content and the tree-level spectrum. A linear gauge-invariant [superpotential](../../../../../superpotential.md) term needs a gauge-singlet [chiral superfield](../../../../../chiral-superfield.md), which the minimal model does not contain. Moreover, with canonical kinetic terms and purely neutral [F-term](../../../../../f-term.md) breaking, without [D-term](../../../../../d-term.md) mass shifts, the [MSSM tree-level sfermion mass constraint](../../../../../mssm-tree-level-sfermion-mass-constraint.md) applies separately to conserved charge sectors. For one electron pair it gives $m_{\tilde e_1}^2+m_{\tilde e_2}^2=2m_e^2$: both scalar partners cannot be heavy. This is an illustrative charge-sector consequence under those assumptions, not an unrestricted inference from the total [supertrace](../../../../../supertrace.md) alone. A separate [hidden supersymmetry-breaking sector](../../../../../hidden-supersymmetry-breaking-sector.md) communicating effective [soft supersymmetry breaking](../../../../../soft-supersymmetry-breaking.md) through loops or suppressed operators avoids the direct canonical tree-level obstruction.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
