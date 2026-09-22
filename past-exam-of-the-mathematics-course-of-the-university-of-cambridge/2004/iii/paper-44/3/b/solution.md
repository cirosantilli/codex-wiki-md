<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the specified $1/\sqrt{2E_{\mathbf p}}$ mode normalization, the [canonical anticommutation relations](../../../../../../canonical-anticommutation-relations.md) are

$$
\boxed{\{a_{\mathbf p}^{s},a_{\mathbf q}^{r\dagger}\}
=\{b_{\mathbf p}^{s},b_{\mathbf q}^{r\dagger}\}
=(2\pi)^3\delta^{sr}\delta^3(\mathbf p-\mathbf q),}
$$

and every other [anticommutator](../../../../../../anticommutator.md) of the $a,b$ operators vanishes. For the [Dirac field](../../../../../../dirac-field.md), they imply the [Equal-time canonical anticommutator of a Dirac field](../../../../../../equal-time-canonical-anticommutator-of-a-dirac-field.md)

$$
\{\psi_\alpha(t,\mathbf x),\psi_\beta^\dagger(t,\mathbf y)\}
=\delta_{\alpha\beta}\delta^3(\mathbf x-\mathbf y),\qquad
\{\psi_\alpha(t,\mathbf x),\psi_\beta(t,\mathbf y)\}=0.
$$

To check the normalization, the two sectors contribute $u(\mathbf p)u^\dagger(\mathbf p)$ and $v(\mathbf p)v^\dagger(\mathbf p)$ with opposite spatial Fourier signs. Reverse $\mathbf p$ in the second contribution. The completeness relations then give

$$
\sum_s\left[u_s(\mathbf p)u_s^\dagger(\mathbf p)
+v_s(-\mathbf p)v_s^\dagger(-\mathbf p)\right]
=\left[(\not p+m)+(\not{\tilde p}-m)\right]\gamma^0
=2E_{\mathbf p}I,
$$

where $\tilde p=(E_{\mathbf p},-\mathbf p)$. This cancels the mode denominator and leaves the Fourier representation of the delta function. Same-momentum $u^\dagger v$ orthogonality must not be used in place of this reversed-momentum identity.

For arbitrary spacetime points,

$$
\{\psi_\alpha(x),\bar\psi_\beta(y)\}
=(i\not\partial_x+m)_{\alpha\beta}\Delta(x-y),
\qquad
\Delta(z)=\int\frac{d^3p}{(2\pi)^3\,2E_{\mathbf p}}
\left(e^{-ip\cdot z}-e^{ip\cdot z}\right).
$$

For spacelike $z$, choose a Lorentz frame with $z^0=0$; reversing spatial [momentum](../../../../../../momentum.md) shows $\Delta(z)=0$. Its derivatives vanish there as well, so the field [anticommutators](../../../../../../anticommutator.md) vanish at spacelike separation. This is fermionic [microcausality](../../../../../../microcausality.md). The anticommutation rules make the occupation of each normalized mode zero or one, implementing the [Pauli exclusion principle](../../../../../../pauli-exclusion-principle.md), and make the [normal-ordered](../../../../../../normal-ordering.md) free [Hamiltonian](../../../../../../hamiltonian.md) positive for both particle sectors.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
