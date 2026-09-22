<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Direct multiplication of the [gamma matrices](../../../../../gamma-matrices.md) in the [chiral representation](../../../../../chiral-gamma-matrix-representation.md) gives

$$
\boxed{\gamma^5=i\gamma^0\gamma^1\gamma^2\gamma^3=
\begin{pmatrix}-I_2&0\\0&I_2\end{pmatrix}}.
$$

For example $\sigma^1\sigma^2\sigma^3=iI_2$ by the [Pauli matrix multiplication law](../../../../../pauli-matrix-multiplication-law.md), and the block multiplications give the displayed signs. Every $\gamma^\mu$ is off-diagonal in this representation, whereas the [chirality matrix](../../../../../chirality-matrix.md) has opposite diagonal blocks. Therefore $\gamma^5\gamma^\mu+\gamma^\mu\gamma^5=0$ for all $\mu$.

The left-handed [chirality](../../../../../chirality-physics.md) condition makes the plane-wave coefficient $\lambda(p)=\binom{\chi}{0}$. With $p\cdot x=Ex^0-\mathbf p\cdot\mathbf x$, the [Dirac equation](../../../../../dirac-equation.md) gives

$$
\not p\,\lambda(p)=0
\quad\Longleftrightarrow\quad
(EI_2+\boldsymbol\sigma\cdot\mathbf p)\chi=0.
$$

Since $(\boldsymbol\sigma\cdot\mathbf p)^2=|\mathbf p|^2I_2$, its [determinant](../../../../../determinant.md) is $E^2-|\mathbf p|^2$. A nonzero [spinor](../../../../../spinor.md) therefore exists exactly when

$$
\boxed{p^2=0}.
$$

For nonzero [momentum](../../../../../momentum.md), put $r=|\mathbf p|$ and write its direction as $(\sin\vartheta\cos\varphi,\sin\vartheta\sin\varphi,\cos\vartheta)$. Normalized [eigenvectors](../../../../../eigenvector.md) of $\boldsymbol\sigma\cdot\widehat{\mathbf p}$ are

$$
\chi_-=
\begin{pmatrix}-e^{-i\varphi}\sin(\vartheta/2)\\\cos(\vartheta/2)\end{pmatrix},
\qquad
\chi_+=\begin{pmatrix}\cos(\vartheta/2)\\e^{i\varphi}\sin(\vartheta/2)\end{pmatrix}.
$$

The general nonzero solution is $\lambda(p)=C\binom{\chi_-}{0}$ for $E=r$ and $\lambda(p)=C\binom{\chi_+}{0}$ for $E=-r$, with arbitrary nonzero complex normalization $C$. At $p=0$ any constant two-component $\chi$ solves the equation, but the [momentum](../../../../../momentum.md) direction and [helicity](../../../../../helicity.md) are undefined. For the physical positive-energy branch this is the [left-handed massless plane-wave spinor](../../../../../left-handed-massless-plane-wave-spinor.md).

A rotation by angle $\alpha$ about $\widehat{\mathbf p}$ acts on the two-component [spinor](../../../../../spinor.md) as

$$
S(R)=e^{-i\alpha\boldsymbol\sigma\cdot\widehat{\mathbf p}/2}.
$$

The plane-wave argument is unchanged because the rotation fixes $\mathbf p$, and $S(R)\chi_-=e^{i\alpha/2}\chi_-$. Thus the positive-energy solution has [helicity](../../../../../helicity.md) $h=-1/2$, where a helicity-$h$ state has rotation phase $e^{-i\alpha h}$. The negative-energy coefficient has the opposite [spinor](../../../../../spinor.md) phase.

In a quantized complex left-handed [Weyl field](../../../../../weyl-field.md), the positive-frequency term annihilates particles and the negative-frequency term creates antiparticles. Reinterpreting negative energy also reverses its spatial [momentum](../../../../../momentum.md); for the positive physical [momentum](../../../../../momentum.md) the two [spinor](../../../../../spinor.md) coefficients have the same left-chiral kernel. Because one multiplies an [annihilation operator](../../../../../annihilation-operator.md) and the other a [creation operator](../../../../../creation-operator.md), the corresponding particle and antiparticle state phases are conjugate. The [helicity content of a quantized Weyl field](../../../../../helicity-content-of-a-quantized-weyl-field.md) is consequently

$$
\boxed{h_{\rm particle}=-\tfrac12,\qquad h_{\rm antiparticle}=+\tfrac12}.
$$

There is one particle spin state at each nonzero [momentum](../../../../../momentum.md), rather than the two helicities supplied by a full massless [Dirac field](../../../../../dirac-field.md). The right-handed [Weyl field](../../../../../weyl-field.md) interchanges these signs. This is the massless relation between [chirality](../../../../../chirality-physics.md) and [helicity](../../../../../helicity.md); it does not identify them for a massive field.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
