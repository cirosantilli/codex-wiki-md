<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The supplied [gamma matrices](../../../../../gamma-matrices.md) use the mostly-minus [metric signature](../../../../../metric-signature.md). The [Pauli matrix multiplication law](../../../../../pauli-matrix-multiplication-law.md) gives $\sigma^1\sigma^2\sigma^3=iI_2$, hence block multiplication yields

$$
\boxed{\gamma^5=i\gamma^0\gamma^1\gamma^2\gamma^3=\begin{pmatrix}-I_2&0\\0&I_2\end{pmatrix}.}
$$

The off-diagonal blocks of every $\gamma^\mu$ connect opposite eigenspaces of this diagonal matrix. Explicitly,

$$
\gamma^5\gamma^0=\begin{pmatrix}0&-I_2\\I_2&0\end{pmatrix}
=-\gamma^0\gamma^5,\qquad
\gamma^5\gamma^i=\begin{pmatrix}0&-\sigma^i\\-\sigma^i&0\end{pmatrix}
=-\gamma^i\gamma^5.
$$

Thus $\{\gamma^5,\gamma^\mu\}=0$, and $(\gamma^5)^2=I_4$. The [chiral projectors](../../../../../chiral-projector.md) $(1\mp\gamma^5)/2$ select the upper and lower two-component blocks, respectively.

Write the [Dirac spinor](../../../../../dirac-spinor.md) as $\psi=(\chi_L,\chi_R)^T$. Substituting the block matrices into the [massless Dirac equation](../../../../../massless-dirac-equation.md) gives two independent [Weyl spinor](../../../../../weyl-spinor.md) equations:

$$
\boxed{i(\partial_t-\boldsymbol\sigma\cdot\boldsymbol\nabla)\chi_L=0,\qquad
i(\partial_t+\boldsymbol\sigma\cdot\boldsymbol\nabla)\chi_R=0.}
$$

They are decoupled because the mass term, which would join the two [chirality](../../../../../chirality-physics.md) components, is absent.

For a left-handed [plane wave](../../../../../plane-wave.md), use $p\cdot x=p^0t-\mathbf p\cdot\mathbf x$. Its coefficient $\xi$ obeys

$$
(p^0I_2+\boldsymbol\sigma\cdot\mathbf p)\xi=0.
$$

Since $(\boldsymbol\sigma\cdot\mathbf p)^2=|\mathbf p|^2 I_2$, the determinant is $(p^0)^2-|\mathbf p|^2$. A nonzero coefficient therefore requires the massless [mass shell](../../../../../mass-shell.md) $\boxed{p^2=0}$. For positive energy and nonzero $\mathbf p$, put $P=|\mathbf p|=p^0$ and parameterize its direction by angles $\vartheta,\varphi$. Then

$$
\boldsymbol\sigma\cdot\widehat{\mathbf p}
=\begin{pmatrix}\cos\vartheta&e^{-i\varphi}\sin\vartheta\\e^{i\varphi}\sin\vartheta&-\cos\vartheta\end{pmatrix},
\qquad
\chi_-=
\begin{pmatrix}-e^{-i\varphi}\sin(\vartheta/2)\\\cos(\vartheta/2)\end{pmatrix}.
$$

Multiplication gives $(\boldsymbol\sigma\cdot\widehat{\mathbf p})\chi_-=-\chi_-$ and $\chi_-^\dagger\chi_-=1$. Hence the [left-handed massless plane-wave spinor](../../../../../left-handed-massless-plane-wave-spinor.md) can be written

$$
\boxed{\lambda_L(p)=N(p)\begin{pmatrix}-e^{-i\varphi}\sin(\vartheta/2)\\\cos(\vartheta/2)\\0\\0\end{pmatrix},\qquad
\psi_L(x)=\lambda_L(p)e^{-ip\cdot x}.}
$$

Here $N(p)$ is an arbitrary complex normalization; $|N|=\sqrt{2P}$ gives $\lambda_L^\dagger\lambda_L=2P$. Away from the negative $z$ axis one can equivalently take

$$
\chi_-=
\frac1{\sqrt{2P(P+p_z)}}\begin{pmatrix}-p_x+ip_y\\P+p_z\end{pmatrix}.
$$

At $\mathbf p=-P\widehat{\mathbf z}$ choose $(1,0)^T$ instead. These are phase patches for the same one-dimensional kernel. The other frequency branch $p^0=-P$ uses the positive eigenvector $\chi_+=(\cos(\vartheta/2),e^{i\varphi}\sin(\vartheta/2))^T$ for the direction of $\mathbf p$. At $p^\mu=0$, the algebraic equation vanishes and any two-component coefficient is possible, but no momentum direction or [helicity](../../../../../helicity.md) is defined there.

A spatial rotation by $\alpha$ about $\widehat{\mathbf p}$ acts on the two-component coefficient by $\exp(-i\alpha\boldsymbol\sigma\cdot\widehat{\mathbf p}/2)$. The negative eigenvector therefore acquires the phase $e^{i\alpha/2}$. Since a state with [helicity](../../../../../helicity.md) $h$ acquires $e^{-i\alpha h}$, the positive-energy left-handed particle has $\boxed{h=-1/2}$. There is only one such spin state at a fixed nonzero momentum, rather than two independent polarizations of the same chiral particle.

The [helicity content of a quantized Weyl field](../../../../../helicity-content-of-a-quantized-weyl-field.md) also includes an antiparticle with opposite [helicity](../../../../../helicity.md). In the field expansion, the negative-frequency term multiplies an antiparticle [fermionic creation operator](../../../../../fermionic-creation-operator.md), while the positive-frequency term multiplies a particle [fermionic annihilation operator](../../../../../fermionic-annihilation-operator.md). Their adjoint roles give conjugate phases for the corresponding created states, so **a left-handed field creates particles with $h=-1/2$ and antiparticles with $h=+1/2$**. The right-handed [Weyl spinor](../../../../../weyl-spinor.md) has the opposite assignments. Quantizing the full massless [Dirac field](../../../../../dirac-field.md), rather than one chiral component, therefore gives both particle helicities and both antiparticle helicities; every excitation has spin one-half, while chirality determines the helicity of each massless sector.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
