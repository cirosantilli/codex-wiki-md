<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the [Minkowski metric](../../../../../minkowski-metric.md) $g^{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$ and [Feynman slash notation](../../../../../feynman-slash-notation.md) $\not p=\gamma^\mu p_\mu$. The [Pauli matrices](../../../../../pauli-matrices.md) satisfy $\sigma_j\sigma_k+\sigma_k\sigma_j=2\delta_{jk}I_2$. In the [Dirac representation of the gamma matrices](../../../../../dirac-representation-of-the-gamma-matrices.md), direct block multiplication gives

$$
(\gamma^0)^2=I_4,\qquad \gamma^0\gamma^j=\begin{pmatrix}0&\sigma_j\\\sigma_j&0\end{pmatrix}=-\gamma^j\gamma^0,
$$

and

$$
\gamma^j\gamma^k=\begin{pmatrix}-\sigma_j\sigma_k&0\\0&-\sigma_j\sigma_k\end{pmatrix}.
$$

Thus the spatial [anticommutators](../../../../../anticommutator.md) are $-2\delta_{jk}I_4$, proving **the Clifford relations**

$$
\boxed{\{\gamma^\mu,\gamma^\nu\}=2g^{\mu\nu}I_4.}
$$

Since partial derivatives commute, their symmetric product selects the symmetric part of the [gamma matrices](../../../../../gamma-matrices.md). Multiplying the [Dirac equation](../../../../../dirac-equation.md) by $i\gamma^\mu\partial_\mu+m$ gives

$$
(i\not\partial+m)(i\not\partial-m)\psi
=(-\gamma^\mu\gamma^\nu\partial_\mu\partial_\nu-m^2)\psi
=-(\Box+m^2)\psi=0.
$$

Hence **every spinor component satisfies the Klein-Gordon equation** with the same mass.

For [parity](../../../../../parity.md), let $x_P=(t,-\mathbf x)$ and $\psi_P(x)=\gamma^0\psi(x_P)$. The chain rule gives $\partial_0\psi(x_P)=(\partial_0\psi)(x_P)$ and $\partial_j\psi(x_P)=-(\partial_j\psi)(x_P)$. Combining these signs with $\gamma^j\gamma^0=-\gamma^0\gamma^j$ proves

$$
(i\not\partial-m)\psi_P(x)
=\gamma^0[(i\not\partial-m)\psi](x_P)=0.
$$

This establishes [parity symmetry in quantum field theory](../../../../../parity-symmetry-in-quantum-field-theory.md) for the free [Dirac equation](../../../../../dirac-equation.md), rather than merely asserting its covariance.

A positive-energy [plane wave](../../../../../plane-wave.md) $\psi=u(p)e^{-ip\cdot x}$ solves $(\not p-m)u=0$. Write $u=(\chi,\eta)^T$. The two block equations are

$$
(E_p-m)\chi-(\boldsymbol\sigma\cdot\mathbf p)\eta=0,\qquad
(\boldsymbol\sigma\cdot\mathbf p)\chi-(E_p+m)\eta=0.
$$

The second gives $\eta=(\boldsymbol\sigma\cdot\mathbf p)\chi/(E_p+m)$. In the first, $(\boldsymbol\sigma\cdot\mathbf p)^2=\mathbf p^2 I_2$ and $E_p^2-\mathbf p^2=m^2$ make the remaining coefficient zero. There are two independent two-component choices $\chi_s$, so

$$
\boxed{u_s(p)=\begin{pmatrix}\chi_s\\(\boldsymbol\sigma\cdot\mathbf p)\chi_s/(E_p+m)\end{pmatrix},\qquad \psi_{p,s}(x)=u_s(p)e^{-ip\cdot x}.}
$$

For a massive [Dirac spinor](../../../../../dirac-spinor.md), choose $\chi_s$ as the two rest-frame [spin](../../../../../spin.md) states along a fixed axis, for example $\sigma_3\chi_s=\pm\chi_s$. The label $s$ distinguishes these canonical [spin](../../../../../spin.md) states after boosting; it is not automatically a [helicity](../../../../../helicity.md) label.

Now $p\cdot x_P=p_P\cdot x$ and $\gamma^0u_s(p)=u_s(p_P)$ for the same fixed $\chi_s$. Therefore

$$
\boxed{\psi_{p,s}(x)\longmapsto\psi_{p_P,s}(x).}
$$

The [parity action on canonical massive spin states](../../../../../parity-action-on-canonical-massive-spin-states.md) leaves the canonical [spin](../../../../../spin.md) label unchanged while reversing the [momentum](../../../../../momentum.md). [Spin](../../../../../spin.md) is an axial vector under [parity](../../../../../parity.md); its orientation is unchanged. Consequently [helicity](../../../../../helicity.md), the projection of [spin](../../../../../spin.md) along [momentum](../../../../../momentum.md), reverses. If $s$ had instead been chosen to denote [helicity](../../../../../helicity.md), the transformed label would have the opposite sign.

The [Dirac adjoint](../../../../../dirac-adjoint.md) is $\bar\psi=\psi^\dagger\gamma^0$, with $\gamma^{0\dagger}=\gamma^0$. Thus

$$
\bar\psi_P(x)=[\gamma^0\psi(x_P)]^\dagger\gamma^0=\psi^\dagger(x_P)=\bar\psi(x_P)\gamma^0.
$$

The [chirality matrix](../../../../../chirality-matrix.md) has $\gamma^5=i\gamma^0\gamma^1\gamma^2\gamma^3=\begin{pmatrix}0&I_2\\I_2&0\end{pmatrix}$ in this representation, so $(\gamma^5)^2=I_4$ and it anticommutes with every $\gamma^\mu$. In particular $\gamma^0\gamma^5\gamma^0=-\gamma^5$. The [parity transformation of a Dirac bilinear](../../../../../parity-transformation-of-a-dirac-bilinear.md) therefore yields

$$
\boxed{\bar\psi_P(x)\psi_P(x)=\bar\psi(x_P)\psi(x_P),\qquad
\bar\psi_P(x)\gamma^5\psi_P(x)=-\bar\psi(x_P)\gamma^5\psi(x_P).}
$$

The first bilinear is a scalar under [parity](../../../../../parity.md), whereas the second is a [pseudoscalar](../../../../../pseudoscalar.md).

For the requested [gamma matrix trace identities](../../../../../gamma-matrix-trace-identities.md), use the [cyclic property of the trace](../../../../../cyclic-property-of-the-trace.md). Conjugation of a product of $n$ [gamma matrices](../../../../../gamma-matrices.md) by $\gamma^5$ multiplies it by $(-1)^n$, but leaves its [trace](../../../../../matrix-trace.md) unchanged. All odd products therefore have zero [trace](../../../../../matrix-trace.md). Taking the [trace](../../../../../matrix-trace.md) of the [Clifford algebra](../../../../../clifford-algebra.md) relation and using $\operatorname{Tr}I_4=4$ gives $\operatorname{Tr}(\gamma^\alpha\gamma^\beta)=4g^{\alpha\beta}$. For four factors, move the first [gamma matrix](../../../../../gamma-matrices.md) successively past the next three using the [anticommutators](../../../../../anticommutator.md). If $A=\operatorname{Tr}(\gamma^\alpha\gamma^\beta\gamma^\rho\gamma^\delta)$, this gives

$$
A=2g^{\alpha\beta}\operatorname{Tr}(\gamma^\rho\gamma^\delta)
-2g^{\alpha\rho}\operatorname{Tr}(\gamma^\beta\gamma^\delta)
+2g^{\alpha\delta}\operatorname{Tr}(\gamma^\beta\gamma^\rho)-A.
$$

Thus $A=4(g^{\alpha\beta}g^{\rho\delta}-g^{\alpha\rho}g^{\beta\delta}+g^{\alpha\delta}g^{\beta\rho})$. Contracting with the relevant [four-vectors](../../../../../four-vector.md) proves all four answers:

$$
\boxed{\begin{aligned}
\operatorname{Tr}(\not p)&=0,\\
\operatorname{Tr}(\not p\not q)&=4p\cdot q,\\
\operatorname{Tr}(\not p\not q\not k)&=0,\\
\operatorname{Tr}(\not p\gamma^\mu\not q\gamma^\nu)&=4[p^\mu q^\nu+p^\nu q^\mu-(p\cdot q)g^{\mu\nu}].
\end{aligned}}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
