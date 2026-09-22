<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The equilibrium quantities $\rho,p,\mathbf B,\Phi$ are real, and the gravitational [Hessian](../../../../../../hessian-matrix.md) $\Phi_{,ij}=\partial_i\partial_j\Phi$ is symmetric. The crucial [tensor](../../../../../../tensor.md) property is

$$
\boxed{V_{ijkl}=V_{klij}.}
$$

This follows directly from the displayed expression for $V$: the products $\delta_{ij}\delta_{kl}$ and $\delta_{il}\delta_{jk}$ are unchanged by interchanging the pairs $(i,j)$ and $(k,l)$; $B_jB_l\delta_{ik}$ is also unchanged; and the two terms involving $B_iB_j\delta_{kl}$ and $B_kB_l\delta_{ij}$ exchange with each other. All coefficients are real.

Multiply $F\boldsymbol\xi$ by $\rho\boldsymbol\eta^*$ and integrate by parts over all space. For admissible [displacement](../../../../../../displacement.md) fields, the boundary contribution at infinity vanishes: the fluid [pressure](../../../../../../pressure.md) and density are confined to the body, and the magnetic stress decays in the surrounding conducting medium. The conducting exterior is included in the integration. For a piecewise description, the usual [displacement](../../../../../../displacement.md) and traction matching conditions cancel the two opposite interface contributions; alternatively, take a smooth transition and then its limit. Thus

$$
\langle\boldsymbol\eta,F\boldsymbol\xi\rangle=-\int\rho\eta_i^*\Phi_{,ij}\xi_j\,dV-\int(\partial_j\eta_i^*)V_{ijkl}(\partial_l\xi_k)\,dV.
$$

The first term is a Hermitian pairing because $\Phi_{,ij}=\Phi_{,ji}$, and the second is Hermitian because $V_{ijkl}=V_{klij}$. Taking the complex conjugate of the same expression with $\boldsymbol\eta$ and $\boldsymbol\xi$ interchanged and relabelling $(i,j)\leftrightarrow(k,l)$ reproduces it. Hence

$$
\boxed{\langle\boldsymbol\eta,F\boldsymbol\xi\rangle=\langle F\boldsymbol\eta,\boldsymbol\xi\rangle.}
$$

This establishes the required [self-adjoint operator](../../../../../../self-adjoint-operator.md) identity in the mass-weighted [inner product](../../../../../../inner-product.md), on the physical [displacement](../../../../../../displacement.md) domain with the stated decay and interface conditions. The negligible-density exterior can be treated as a small-positive-density conducting limit when defining this weighted pairing; its magnetic contribution is retained even as its inertia becomes negligible.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
