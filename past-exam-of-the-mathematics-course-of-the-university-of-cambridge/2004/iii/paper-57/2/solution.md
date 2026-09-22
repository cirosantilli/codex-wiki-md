<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An [orthonormal tetrad](../../../../../orthonormal-frame-in-spacetime.md), or [vierbein](../../../../../orthonormal-coframe-in-spacetime.md), is a local basis $e_I{}^a$ of tangent vectors together with inverse coframe $e_a{}^I$, satisfying $g_{ab}e_I{}^ae_J{}^b=\eta_{IJ}$ and $g_{ab}=e_a{}^Ie_b{}^J\eta_{IJ}$. Capital indices label the locally orthonormal Lorentz frame; lower-case indices label spacetime coordinates. Changing the frame by a local [Lorentz transformation](../../../../../lorentz-transformation.md) leaves the metric unchanged. A [spinor](../../../../../spinor.md) description uses a compatible local spin frame and the torsion-free [spin connection](../../../../../spin-connection.md).

Let fixed flat matrices satisfy $\{\Gamma_I,\Gamma_J\}=2\eta_{IJ}\mathbf1$. The [curved spacetime gamma matrices](../../../../../curved-spacetime-gamma-matrices.md) are $\gamma_a=e_a{}^I\Gamma_I$ and $\gamma^a=e_I{}^a\Gamma^I$. Therefore

$$
\boxed{\{\gamma_a,\gamma_b\}=e_a{}^Ie_b{}^J\{\Gamma_I,\Gamma_J\}=2g_{ab}\mathbf1.}
$$

The identity matrix is four by four for a four-dimensional [Dirac spinor](../../../../../dirac-spinor.md). The combined tensor/spin [covariant derivative](../../../../../covariant-derivative.md) makes $\nabla_a\gamma_b=0$, the Clifford version of the [tetrad postulate](../../../../../tetrad-postulate.md).

Fix the curvature slots by $R_{abcd}=g_{ae}R^e{}_{bcd}$, with $[\nabla_c,\nabla_d]v^a=R^a{}_{bcd}v^b$, and $R=g^{ac}g^{bd}R_{abcd}$. The torsion-free [spin connection](../../../../../spin-connection.md) then has $[\nabla_a,\nabla_b]\psi=\tfrac14R_{abcd}\gamma^c\gamma^d\psi$. These choices fix the signs in the requested identities.

Write $\gamma^{ab}=\gamma^{[a}\gamma^{b]}$ and similarly for four indices. Clifford anticommutation gives

$$
\begin{aligned}
\gamma^a\gamma^b\gamma^c\gamma^d={}&\gamma^{abcd}+g^{ab}\gamma^{cd}-g^{ac}\gamma^{bd}+g^{ad}\gamma^{bc}\\
&+g^{bc}\gamma^{ad}-g^{bd}\gamma^{ac}+g^{cd}\gamma^{ab}\\
&+(g^{ab}g^{cd}-g^{ac}g^{bd}+g^{ad}g^{bc})\mathbf1.
\end{aligned}
$$

On contraction with the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md), the four-form term vanishes by the [first Bianchi identity](../../../../../first-bianchi-identity.md). The first and last two-form terms vanish by pair antisymmetry; the remaining two-form terms are symmetric Ricci contractions against antisymmetric gamma matrices and vanish too. The scalar terms are zero, minus R and minus R respectively. Thus the [Riemann tensor Clifford contraction](../../../../../riemann-tensor-clifford-contraction.md) is

$$
\boxed{R_{abcd}\gamma^a\gamma^b\gamma^c\gamma^d=-2R\mathbf1.}
$$

This algebraic result is independent of Lorentz signature when the contraction convention is held fixed.

Apply the Dirac operator twice, using covariant constancy of the gamma matrices. Define the rough wave operator by $\Box=g^{ab}\nabla_a\nabla_b$, with the full connection acting on the intermediate covector-spinor derivative. Splitting the product into symmetric and antisymmetric parts gives

$$
\begin{aligned}
(\gamma^a\nabla_a)^2\psi&=\Box\psi+\frac12\gamma^{ab}[\nabla_a,\nabla_b]\psi\\
&=\Box\psi+\frac18R_{abcd}\gamma^a\gamma^b\gamma^c\gamma^d\psi=(\Box-R/4)\psi.
\end{aligned}
$$

Consequently the [Lichnerowicz spinor-square formula](../../../../../lichnerowicz-spinor-square-formula.md) and the assumed massless [Dirac equation](../../../../../dirac-equation.md) imply $\boxed{(\Box-R/4)\psi=0}$. Torsion would modify the commutator and introduce extra terms, so the [torsion-free connection](../../../../../torsion-free-connection.md) is part of this argument.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
