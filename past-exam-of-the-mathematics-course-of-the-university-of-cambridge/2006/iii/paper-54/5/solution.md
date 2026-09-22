<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Choose canonical vector normalization, $g>0$, and the convention that the [Fayet–Iliopoulos term](../../../../../fayet-iliopoulos-term.md) contributes $+\xi D$. In a constant Lorentz-invariant vacuum with vanishing gauge field strength, the [gaugino](../../../../../gaugino.md) transformation contains

$$
\delta\lambda_\alpha=i\epsilon_\alpha\langle D\rangle.
$$

A nonzero $\langle D\rangle$ therefore shifts a fermion by a constant under [supersymmetry](../../../../../supersymmetry-split.md): no invariant vacuum can have this expectation. With only D-term breaking, the [Goldstino](../../../../../goldstino.md) is the gaugino $\lambda$. If F-term expectation values were present too, the Goldstino would instead be the corresponding linear combination of matter fermions and gauginos.

For a genuinely charged single [chiral superfield](../../../../../chiral-superfield.md), $q\ne0$, gauge invariance forbids every nonconstant polynomial superpotential in that field. The renormalizable [superspace](../../../../../superspace.md) action is consequently

$$
S=\int d^4x\left\{\int d^4\theta\,\Phi^\dagger e^{2gqV}\Phi
+\left[\frac14\int d^2\theta\,\mathcal W^\alpha\mathcal W_\alpha+\mathrm{h.c.}\right]
+2\xi\int d^4\theta\,V\right\},
$$

where $\mathcal W_\alpha=-\bar D^2D_\alpha V/4$. A constant superpotential is dynamically irrelevant in global supersymmetry. Take the standard vector expansion with highest component $\theta^2\bar\theta^2D/2$. In the matter exponential, the term $2gqV$ then contributes $gq|\phi|^2D$. The gauge kinetic chiral integral contributes $D^2/2$, and the FI term contributes $\xi D$. Thus

$$
\mathcal L_{\rm aux}=F^*F+\frac12D^2+D(gq|\phi|^2+\xi).
$$

The auxiliary equations are $F=0$ and $D=-(gq|\phi|^2+\xi)$. Completing the square gives

$$
\mathcal L_D=\frac12\bigl[D+gq|\phi|^2+\xi\bigr]^2-\frac12(gq|\phi|^2+\xi)^2,
\qquad\boxed{V_D=\frac12(gq|\phi|^2+\xi)^2.}
$$

This is the [single charged-field D-term breaking](../../../../../single-charged-field-d-term-breaking.md) model. Its vacuum is found by minimizing over $\rho=|\phi|^2\geq0$, not by assuming that a nonzero FI constant must break supersymmetry.

For $q\xi>0$, the square cannot be canceled by any $\rho\geq0$. It is minimized at the origin, where

$$
\boxed{\langle\phi\rangle=0,\quad\langle D\rangle=-\xi,\quad V_{\min}=\xi^2/2>0.}
$$

[Supersymmetry breaking](../../../../../supersymmetry-breaking.md) occurs while the internal $U(1)$ [gauge symmetry](../../../../../gauge-invariance.md) remains unbroken. Expanding the [scalar potential](../../../../../scalar-potential.md) about the origin gives

$$
V_D=\frac12\xi^2+gq\xi|\phi|^2+\frac12g^2q^2|\phi|^4.
$$

There is no superpotential fermion mass and no gaugino-matter mixing at $\phi=0$. Therefore the chiral multiplet mass splitting is

$$
\boxed{m_\phi^2=gq\xi,\qquad m_\psi=0,\qquad\Delta m^2=gq\xi.}
$$

Both real components of the complex scalar have the same positive squared mass; the gaugino is the massless [Goldstino](../../../../../goldstino.md). With this sign convention and $\xi>0$, the breaking condition is $q>0$. Reversing the FI sign convention reverses this quoted charge inequality, while the condition that the scalar cannot cancel the auxiliary-field shift is unchanged.

For $q\xi<0$, the minimum instead satisfies

$$
\boxed{|\langle\phi\rangle|^2=-\frac{\xi}{gq},\qquad\langle D\rangle=0,\qquad V_{\min}=0.}
$$

The nonzero charged scalar expectation breaks the continuous internal gauge symmetry and preserves [supersymmetry](../../../../../supersymmetry-split.md). To see the resulting [supersymmetric Higgs mechanism](../../../../../supersymmetric-higgs-mechanism.md), choose a real representative $v>0$ and expand $\phi=v+(h+ia)/\sqrt2$. The scalar kinetic term supplies a vector mass, the D-term potential supplies the radial scalar mass, and the Yukawa interaction $-\sqrt2gq\phi^*\lambda\psi+\mathrm{h.c.}$ pairs the two Weyl fermions. They have the common squared mass

$$
\boxed{m_A^2=m_h^2=m_{\lambda\psi}^2=2g^2q^2v^2=-2gq\xi.}
$$

The phase field $a$ is the absorbed Goldstone mode. There is no Goldstino in this supersymmetric Higgs vacuum; the fields assemble into a [massive N=1 vector multiplet](../../../../../massive-n-1-vector-multiplet.md). This branch makes explicit that internal gauge breaking and supersymmetry breaking are different phenomena.

If $\xi=0$ and $q\ne0$, the minimum of $g^2q^2|\phi|^4/2$ is $\phi=0$. **Both supersymmetry and the continuous gauge symmetry are then unbroken**, and the fields have zero tree-level masses at that vacuum. For the degenerate uncharged case $q=0$ with no superpotential interactions, a nonzero $\xi$ still breaks supersymmetry in the vector sector, but the free chiral multiplet stays unsplit and cannot Higgs the gauge field. An uncharged field would allow additional superpotential terms, outside the genuinely charged model above.

The calculation is classical. A single charged Weyl fermion has nonzero Abelian gauge and mixed gravitational anomaly coefficients proportional to $q^3$ and $q$; a complete quantum gauge theory needs an anomaly-canceling completion. The tree-level branches above refer to the specified field content; extra fields in such a completion can change the vacuum structure.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
