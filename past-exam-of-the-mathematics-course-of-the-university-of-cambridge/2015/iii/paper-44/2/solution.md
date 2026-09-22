<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a differentiable curve $R(t)$ in the [SO(3) group](../../../../../so-3-group.md) with $R(0)=I$, differentiating $R(t)^TR(t)=I$ gives $X^T+X=0$, where $X=R'(0)$. Conversely, if $X$ is a real [skew-symmetric matrix](../../../../../skew-symmetric-matrix.md), $e^{tX}$ is an [orthogonal matrix](../../../../../orthogonal-matrix.md) and has [determinant](../../../../../determinant.md) $e^{t\operatorname{tr}X}=1$. Hence

$$
\boxed{\mathfrak{so}(3)=\{X\in M_3(\mathbb R):X^T=-X\},\qquad\dim\mathfrak{so}(3)=3.}
$$

The displayed generators of the [SO(3) Lie algebra](../../../../../so-3-lie-algebra.md) are

$$
T_1=\begin{pmatrix}0&0&0\\0&0&-1\\0&1&0\end{pmatrix},\quad T_2=\begin{pmatrix}0&0&1\\0&0&0\\-1&0&0\end{pmatrix},\quad T_3=\begin{pmatrix}0&-1&0\\1&0&0\\0&0&0\end{pmatrix}.
$$

They are [linearly independent](../../../../../linear-independence.md) and span the three independent entries of a real [skew-symmetric matrix](../../../../../skew-symmetric-matrix.md). Equivalently, $T_a\mathbf v=\mathbf e_a\times\mathbf v$. The vector triple-product identity then gives

$$
[T_a,T_b]\mathbf v=\mathbf e_a\times(\mathbf e_b\times\mathbf v)-\mathbf e_b\times(\mathbf e_a\times\mathbf v)=(\mathbf e_a\times\mathbf e_b)\times\mathbf v.
$$

Thus the [structure constants of a Lie algebra](../../../../../structure-constant-of-a-lie-algebra.md) in this basis are

$$
\boxed{[T_a,T_b]=\epsilon_{abc}T_c,\qquad f_{ab}{}^c=\epsilon_{abc}.}
$$

Use a real, antisymmetric convention throughout the [SO(3) vector Higgs model](../../../../../so-3-vector-higgs-model.md). With [gauge coupling](../../../../../gauge-coupling.md) $g$, the [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) and [gauge field strength](../../../../../gauge-field-strength.md) are

$$
\boxed{D_\mu\Phi=\partial_\mu\Phi+gA_\mu\Phi,\qquad F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu+g[A_\mu,A_\nu],\qquad[D_\mu,D_\nu]=gF_{\mu\nu}.}
$$

There is no factor of $i$ in these formulas because $T_a$ are real antisymmetric generators. For a local [non-Abelian gauge transformation](../../../../../non-abelian-gauge-transformation.md) $\Phi'=R\Phi$, with $R(x)$ in the [SO(3) group](../../../../../so-3-group.md), the compatible transformation of the [gauge potential](../../../../../gauge-field.md) is

$$
A'_\mu=RA_\mu R^{-1}-g^{-1}(\partial_\mu R)R^{-1}.
$$

It gives $D'_\mu\Phi'=R D_\mu\Phi$ and $F'_{\mu\nu}=RF_{\mu\nu}R^{-1}$. These covariance laws fix the relative signs in the [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) and [gauge field strength](../../../../../gauge-field-strength.md).

An [SO(3) invariant quartic scalar potential](../../../../../so-3-invariant-quartic-scalar-potential.md) is

$$
\boxed{V(\Phi)=\frac\lambda4(\Phi^T\Phi-v^2)^2,\qquad\lambda>0,\quad v>0.}
$$

Since $(R\Phi)^T(R\Phi)=\Phi^T\Phi$, this [scalar potential](../../../../../scalar-potential.md) is [gauge-invariant](../../../../../gauge-invariance.md). Its minimum is the sphere $\Phi^T\Phi=v^2$, rather than a preferred direction in the internal vector space.

Writing $\mathbf A_\mu=(A_{\mu1},A_{\mu2},A_{\mu3})$, the [cross product](../../../../../cross-product.md) form of the [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) is $D_\mu\Phi=\partial_\mu\Phi+g\mathbf A_\mu\times\Phi$. In components this is

$$
\boxed{\begin{aligned}(D_\mu\Phi)_1&=\partial_\mu\Phi_1+g(A_{\mu2}\Phi_3-A_{\mu3}\Phi_2),\\(D_\mu\Phi)_2&=\partial_\mu\Phi_2+g(A_{\mu3}\Phi_1-A_{\mu1}\Phi_3),\\(D_\mu\Phi)_3&=\partial_\mu\Phi_3+g(A_{\mu1}\Phi_2-A_{\mu2}\Phi_1).\end{aligned}}
$$

Correspondingly, the [gauge field strength](../../../../../gauge-field-strength.md) has components

$$
F_{\mu\nu a}=\partial_\mu A_{\nu a}-\partial_\nu A_{\mu a}+g\epsilon_{abc}A_{\mu b}A_{\nu c}.
$$

A [covariantly constant vector Higgs field](../../../../../covariantly-constant-vector-higgs-field.md) has constant norm, because

$$
\partial_\mu(\Phi^T\Phi)=2\Phi^T\partial_\mu\Phi=-2g\Phi^TA_\mu\Phi=0.
$$

The last equality uses antisymmetry of the [gauge potential](../../../../../gauge-field.md). On a connected region write this norm as $\phi\geq0$. If $\phi=0$, the [vector Higgs field](../../../../../vector-higgs-field.md) is identically zero. If $\phi>0$, the [SO(3) group](../../../../../so-3-group.md) acts transitively on [unit vectors](../../../../../unit-vector.md), so choose a smooth local [non-Abelian gauge transformation](../../../../../non-abelian-gauge-transformation.md) rotating $\Phi/\phi$ to $\mathbf e_3$. In this [unitary gauge](../../../../../unitary-gauge.md), $\Phi=(0,0,\phi)^T$ with $\phi$ constant. This is a local construction, and is global on a trivial contractible region; a nontrivial bundle can require more than one gauge patch.

For nonzero $\phi$, substituting the constant aligned [vector Higgs field](../../../../../vector-higgs-field.md) into $D_\mu\Phi=0$ gives $g\phi(A_{\mu2},-A_{\mu1},0)^T=0$. For nonzero [gauge coupling](../../../../../gauge-coupling.md), **the most general compatible [gauge potential](../../../../../gauge-field.md) and [gauge field strength](../../../../../gauge-field-strength.md) are**

$$
\boxed{A_\mu=a_\mu T_3,\qquad F_{\mu\nu}=(\partial_\mu a_\nu-\partial_\nu a_\mu)T_3,}
$$

where $a_\mu$ is an arbitrary real one-form. Thus the surviving [gauge group](../../../../../gauge-group.md) is the $SO(2)$ [stabilizer subgroup](../../../../../stabilizer-subgroup.md) of $\mathbf e_3$. A [covariantly constant vector Higgs field](../../../../../covariantly-constant-vector-higgs-field.md) does not force the [gauge field strength](../../../../../gauge-field-strength.md) to vanish: it only requires the curvature to annihilate that field.

For the [Higgs mechanism](../../../../../higgs-mechanism.md), choose a vacuum of the [SO(3) invariant quartic scalar potential](../../../../../so-3-invariant-quartic-scalar-potential.md), so the constant norm is $v$. The canonically normalized [kinetic term](../../../../../kinetic-term.md) then contains

$$
\frac12(D_\mu\Phi)^T(D^\mu\Phi)\supset\frac12g^2v^2\left(A_{\mu1}A_1^\mu+A_{\mu2}A_2^\mu\right).
$$

The two broken-direction [gauge bosons](../../../../../gauge-boson.md) have mass $gv$ (or $|g|v$ if the sign of $g$ is unrestricted), while the $T_3$ [gauge boson](../../../../../gauge-boson.md) remains massless. The two angular [Goldstone bosons](../../../../../goldstone-boson.md) supply the massive vectors' [longitudinal gauge-boson polarizations](../../../../../longitudinal-polarization-of-a-massive-vector-boson.md). The radial fluctuation remains a physical [scalar field](../../../../../scalar-field.md), with $m_h^2=2\lambda v^2$ for this normalization. The condition $D_\mu\Phi=0$ selects backgrounds without broken-direction [gauge potentials](../../../../../gauge-field.md); fluctuations about such a vacuum exhibit the two massive modes. Constancy of the norm alone does not require it to minimize the [scalar potential](../../../../../scalar-potential.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
