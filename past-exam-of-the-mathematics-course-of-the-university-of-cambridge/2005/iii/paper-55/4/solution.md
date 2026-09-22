<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Take canonical kinetic terms, gauge coupling $g>0$, and a nonzero charge $q$. Define $e=gq$ and choose the convention in which the [Fayet–Iliopoulos term](../../../../../fayet-iliopoulos-term.md) contributes $\xi D$ to the [Lagrangian](../../../../../lagrangian.md). With one charged [chiral superfield](../../../../../chiral-superfield.md), gauge invariance permits no nonconstant polynomial [superpotential](../../../../../superpotential.md); an irrelevant global constant gives $F=0$. The real [auxiliary field](../../../../../auxiliary-field.md) part is

$$
\mathcal L_D=\frac12D^2+D(\xi+e|\phi|^2).
$$

Its equation of motion is $D=-(\xi+e|\phi|^2)$. Eliminating it gives the [D-term scalar potential](../../../../../d-term-scalar-potential.md)

$$
\boxed{V_D=\frac12(\xi+e|\phi|^2)^2.}
$$

The [gaugino](../../../../../gaugino.md) transformation has the form $\delta\lambda=i\epsilon D+$ a field-strength term, with a convention-dependent overall phase. In a translationally invariant vacuum with zero field strength, a nonzero $\langle D\rangle$ therefore gives an inhomogeneous shift of $\lambda$: no nonzero [supersymmetry](../../../../../supersymmetry-split.md) parameter leaves the vacuum invariant. The massless [Goldstino](../../../../../goldstino.md) is consequently the [gaugino](../../../../../gaugino.md), not the matter fermion, since $F=0$.

Minimize the potential over $u=|\phi|^2\geq0$. If $q\xi<0$, the allowed value $u=-\xi/e$ sets $D=0$, so [supersymmetry](../../../../../supersymmetry-split.md) is unbroken while the internal gauge symmetry is Higgsed. If $\xi=0$, the origin also has $D=0$. For the broken branch, $q\xi>0$ and the formal zero of $D$ would require negative $u$. The actual minimum is

$$
\boxed{\langle\phi\rangle=0,\qquad\langle D\rangle=-\xi,
\qquad V_{\min}=\frac12\xi^2>0,
\qquad q\xi>0.}
$$

This is [single charged-field D-term breaking](../../../../../single-charged-field-d-term-breaking.md). Nonzero FI parameter alone does not force breaking if a scalar can cancel it. The degenerate case $q=0$ is different: any $\xi\ne0$ breaks [supersymmetry](../../../../../supersymmetry-split.md) in the vector sector while the neutral scalar remains flat; the sign test above assumes an actually charged field.

Expand around the broken vacuum:

$$
V_D=\frac12\xi^2+e\xi|\phi|^2+\frac12e^2|\phi|^4.
$$

For $\phi=(\phi_R+i\phi_I)/\sqrt2$, both canonically normalized real scalars have squared mass $e\xi=gq\xi>0$. The matter [Weyl spinor](../../../../../weyl-spinor.md) has no [superpotential](../../../../../superpotential.md) mass. The gauge boson remains massless because $\langle\phi\rangle=0$. The gauge Yukawa coupling, proportional to $\phi^*\lambda\psi$, gives no fermion mixing or mass at this vacuum, so the [gaugino](../../../../../gaugino.md) is also massless. The tree-level spectrum is therefore

$$
\begin{array}{c|c}
\text{field}&\text{squared mass}\\\hline
\phi_R,\phi_I&gq\xi\\
\psi&0\\
A_\mu&0\\
\lambda\ \text{(Goldstino)}&0
\end{array}
$$

and the chiral-multiplet splitting is

$$
\boxed{m_{\mathrm{scalar}}^2-m_{\mathrm{fermion}}^2=gq\xi,\qquad
m_{\mathrm{scalar}}=\sqrt{gq\xi}.}
$$

The vector and its [gaugino](../../../../../gaugino.md) happen to remain degenerate at zero mass even though [supersymmetry](../../../../../supersymmetry-split.md) is broken. If the sign convention for the FI contribution is reversed, the sign criterion changes accordingly; the invariant condition is that the scalar condensate cannot cancel the auxiliary source. This is the classical toy-model spectrum; a quantum completion of the single charged-fermion theory also has to cancel its [gauge anomalies](../../../../../gauge-anomaly.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
