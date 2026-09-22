<h1 id="33a/solution">Solution</h1>

↑ **Parent:** [33A](../33a.md)

Every [density operator](../../../../../density-matrix.md) can be written as

$$
\rho=\sum_jp_j|\psi_j\rangle\langle\psi_j|,
\qquad p_j\geq0,
\qquad\sum_jp_j=1.
$$

Therefore $\langle\phi|\rho|\phi\rangle=\sum_jp_j|\langle\psi_j|\phi\rangle|^2\geq0$, so $\rho$ is a [positive semidefinite operator](../../../../../positive-operator.md), and $\operatorname{Tr}\rho=\sum_jp_j=1$. A [pure quantum state](../../../../../pure-state.md) has a rank-one density operator $|\psi\rangle\langle\psi|$, equivalently $\rho^2=\rho$ and $\operatorname{Tr}(\rho^2)=1$. A [mixed quantum state](../../../../../mixed-state.md) is not pure and has $\operatorname{Tr}(\rho^2)<1$ in finite dimension.

The [Von Neumann equation](../../../../../von-neumann-equation.md) and the [Pauli matrix commutator identity](../../../../../pauli-matrix-commutator-identity.md) give

$$
\dot\rho=-\frac{i}{\hbar}[H,\rho],
\qquad
[\boldsymbol\omega\mathbin\cdot\boldsymbol\sigma,
\mathbf a\mathbin\cdot\boldsymbol\sigma]
=2i(\boldsymbol\omega\times\mathbf a)\mathbin\cdot\boldsymbol\sigma,
$$

so the [Bloch vector](../../../../../bloch-vector.md) obeys

$$
\dot{\mathbf a}=2\boldsymbol\omega\times\mathbf a.
$$

Writing $\omega=|\boldsymbol\omega|$ and $\widehat{\boldsymbol\omega}=\boldsymbol\omega/\omega$, the assumption $\mathbf a\mathbin\cdot\boldsymbol\omega=0$ gives

$$
\mathbf a(t)=\mathbf a\cos(2\omega t)
+(\widehat{\boldsymbol\omega}\times\mathbf a)\sin(2\omega t),
$$

and hence

$$
\boxed{\rho(t)=\frac12\left[1_{\mathcal H}+\left(\mathbf a\cos(2\omega t)+(\widehat{\boldsymbol\omega}\times\mathbf a)\sin(2\omega t)\right)\mathbin\cdot\boldsymbol\sigma\right]}.
$$

Unitary evolution rotates the Bloch vector and preserves its length. Since $|\mathbf a|<1$, the state remains mixed, whereas $|\!\uparrow_x\rangle$ has the unit Bloch vector $(1,0,0)$. The system is therefore never definitely in $|\!\uparrow_x\rangle$.

## ↑ Ancestors (10)

1. [33A](../33a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
