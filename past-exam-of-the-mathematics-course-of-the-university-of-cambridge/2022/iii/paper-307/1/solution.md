<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Treating derivatives with respect to the [Grassmann variables](../../../../../grassmann-variable.md) as graded derivatives and using $\{\partial_\alpha,\theta^\beta\}=\delta_\alpha{}^\beta$ gives

$$
\{\mathcal D_\alpha,\overline{\mathcal D}_{\dot\alpha}\}
=-2i\sigma^\mu_{\alpha\dot\alpha}\partial_\mu
=2\sigma^\mu_{\alpha\dot\alpha}\mathcal P_\mu,
\qquad \mathcal P_\mu=-i\partial_\mu.
$$

The terms in $\{\mathcal D_\alpha,\mathcal D_\beta\}$ and $\{\overline{\mathcal D}_{\dot\alpha},\overline{\mathcal D}_{\dot\beta}\}$ cancel pairwise, so both vanish.

A [chiral superfield](../../../../../chiral-superfield.md) obeys $\overline{\mathcal D}_{\dot\alpha}\Phi=0$, while an [antichiral superfield](../../../../../antichiral-superfield.md) obeys $\mathcal D_\alpha\Phi^\dagger=0$. Since $\overline{\mathcal D}_{\dot\alpha}y^\mu=0$ for $y^\mu=x^\mu+i\theta\sigma^\mu\bar\theta$, the general chiral expansion is

$$
\Phi(y,\theta)=\phi(y)+\sqrt2\theta\psi(y)+\theta^2F(y).
$$

In the original coordinates this is

$$
\Phi=\phi+\sqrt2\theta\psi+\theta^2F+i\theta\sigma^\mu\bar\theta\,\partial_\mu\phi
-\frac{i}{\sqrt2}\theta^2\partial_\mu\psi\sigma^\mu\bar\theta
-\frac14\theta^2\bar\theta^2\Box\phi,
$$

with signs following the conventions of the question.

A holomorphic function $W(\Phi)$ is chiral. Its highest component transforms into a spacetime divergence, so the [F-term](../../../../../f-term.md) action

$$
S_W=\int d^4x\,d^2\theta\,W(\Phi)+\mathrm{h.c.}
$$

is supersymmetric even though it integrates over only chiral half of [superspace](../../../../../superspace.md).

The [non-renormalization theorem](../../../../../non-renormalization-theorem.md) says that perturbative loop corrections are full-superspace D-terms and cannot generate a new local superpotential. Holomorphy and spurion symmetries therefore preserve

$$
W_{\rm Wilsonian}=\frac12m\Phi^2+\frac13\lambda\Phi^3.
$$

The Kähler potential is renormalized, however. If its kinetic term is $Z\Phi^\dagger\Phi$, canonical normalization $\Phi_c=Z^{1/2}\Phi$ gives

$$
m_{\rm phys}=\frac mZ,
\qquad
\lambda_{\rm phys}=\frac\lambda{Z^{3/2}},
$$

up to scheme and scale conventions. Thus superpotential parameters are holomorphic invariants while physical masses and couplings still run through [wave-function renormalization](../../../../../wave-function-renormalization.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 307](../../paper-307-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
