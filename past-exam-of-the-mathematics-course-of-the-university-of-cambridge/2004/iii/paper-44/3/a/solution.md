<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use signature $(+,-,-,-)$ and the free [Dirac equation](../../../../../../dirac-equation.md) $(i\gamma^\mu\partial_\mu-m)\psi=0$. For positive $p^0=E_{\mathbf p}=\sqrt{\mathbf p^2+m^2}$, substitution of the two frequency signs gives

$$
\psi=u_s(p)e^{-ip\cdot x}:\quad(\not p-m)u_s(p)=0,
\qquad
\psi=v_s(p)e^{ip\cdot x}:\quad(\not p+m)v_s(p)=0.
$$

Multiplying by the opposite factor shows $p^2=m^2$. Each equation has two independent solutions for a massive field.

In the [Dirac basis](../../../../../../dirac-representation-of-the-gamma-matrices.md), $\gamma^0=\operatorname{diag}(I,-I)$ and $\gamma^i=\begin{pmatrix}0&\sigma_i\\-\sigma_i&0\end{pmatrix}$. For orthonormal two-component [spin](../../../../../../spin.md) labels $\xi_s,\eta_s$, convenient solutions are

$$
\boxed{u_s(p)=\sqrt{E_{\mathbf p}+m}
\begin{pmatrix}\xi_s\\
\dfrac{\boldsymbol\sigma\cdot\mathbf p}{E_{\mathbf p}+m}\xi_s
\end{pmatrix},\qquad
v_s(p)=\sqrt{E_{\mathbf p}+m}
\begin{pmatrix}
\dfrac{\boldsymbol\sigma\cdot\mathbf p}{E_{\mathbf p}+m}\eta_s\\
\eta_s
\end{pmatrix}.}
$$

The two-block equations verify these expressions using $(\boldsymbol\sigma\cdot\mathbf p)^2=\mathbf p^2I$. At rest the positive-frequency solutions have only upper components and the negative-frequency solutions only lower components. Their normalizations are $u_s^\dagger u_r=v_s^\dagger v_r=2E_{\mathbf p}\delta_{sr}$ and $\bar u_su_r=2m\delta_{sr}$, $\bar v_sv_r=-2m\delta_{sr}$. Their completeness relations are

$$
\sum_su_s(p)\bar u_s(p)=\not p+m,\qquad
\sum_sv_s(p)\bar v_s(p)=\not p-m.
$$

The field expansion combines [fermionic annihilation operators](../../../../../../fermionic-annihilation-operator.md) multiplying the positive-frequency waves with [antiparticle](../../../../../../antiparticle.md) [fermionic creation operators](../../../../../../fermionic-creation-operator.md) multiplying the negative-frequency waves. The latter frequency sign is not the [energy](../../../../../../energy.md) of a physical negative-energy [antiparticle](../../../../../../antiparticle.md) state.

## ↑ Ancestors (11)

1. [A](../a.md)
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
