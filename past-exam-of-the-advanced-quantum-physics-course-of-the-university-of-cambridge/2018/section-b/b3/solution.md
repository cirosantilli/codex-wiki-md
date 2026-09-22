<h1 id="section-b/b3/solution">Solution</h1>

↑ **Parent:** [B3](../b3.md)

Take a normalized [spin one-half](../../../../spin-one-half.md) state in the $S_z$ [eigenbasis](../../../../eigenbasis.md). Since $\mathbf S=(\hbar/2)\boldsymbol\sigma$, direct multiplication of the [Pauli matrices](../../../../pauli-matrices.md) gives

$$
\langle S_x\rangle=\frac\hbar2(\alpha^*\beta+\beta^*\alpha),\quad \langle S_y\rangle=\frac\hbar2(-i\alpha^*\beta+i\beta^*\alpha),\quad \langle S_z\rangle=\frac\hbar2(|\alpha|^2-|\beta|^2).
$$

Substitution of the half-angle parametrization gives

$$
\boxed{\langle\mathbf S\rangle=\frac\hbar2(\sin\theta\cos\phi,\sin\theta\sin\phi,\cos\theta).}
$$

Thus $\theta$ and $\phi$ are precisely the polar and azimuthal angles of the mean [spin](../../../../spin.md). Two complex coefficients contain four real parameters; normalization removes one and an unobservable common [quantum phase](../../../../quantum-phase.md) removes another. The resulting pure states form the [Bloch sphere](../../../../bloch-sphere.md). One may choose $\alpha$ real and nonnegative away from the patch where $\alpha=0$. At the poles the azimuth is redundant. The length $|\langle\mathbf S\rangle|=\hbar/2$ should not be confused with $\sqrt{\langle S^2\rangle}=\sqrt3\hbar/2$.

For a spatial [plane wave](../../../../plane-wave.md), $-i\hbar\boldsymbol\nabla$ becomes $\hbar\mathbf k$, so the [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) reduces to the [Weyl Hamiltonian](../../../../weyl-hamiltonian.md) [matrix](../../../../matrix.md)

$$
H(\mathbf k)=\hbar v\,\boldsymbol\sigma\cdot\mathbf k.
$$

Define $\mathbf n=(\sin\theta\cos\phi,\sin\theta\sin\phi,\cos\theta)$ and $\chi_+=(\cos(\theta/2),e^{i\phi}\sin(\theta/2))^{\mathsf T}$. The [matrix](../../../../matrix.md)

$$
\boldsymbol\sigma\cdot\mathbf n=\begin{pmatrix}\cos\theta&e^{-i\phi}\sin\theta\\e^{i\phi}\sin\theta&-\cos\theta\end{pmatrix}
$$

satisfies $(\boldsymbol\sigma\cdot\mathbf n)\chi_+=\chi_+$ by the angle-addition identities. Consequently the displayed [spinor](../../../../spinor.md) is an [energy eigenstate](../../../../energy-eigenstate.md) for either $\mathbf k=+k\mathbf n$ or $\mathbf k=-k\mathbf n$, with respective energies $+\hbar vk$ and $-\hbar vk$, for $k\geq0$. Equivalently, at each fixed nonzero [wavevector](../../../../wavevector.md) the two branches are

$$
\boxed{E_\pm(\mathbf k)=\pm\hbar v|\mathbf k|\quad(v>0).}
$$

If $v<0$, the two [energy](../../../../energy-split.md) labels exchange; the ordered [eigenvalues](../../../../eigenvalue.md) are $\pm\hbar|v||\mathbf k|$. Taking $v>0$ sets the convention in the sketches. An [orthogonal](../../../../orthogonal-vectors.md) [spinor](../../../../spinor.md) $\chi_-=(-e^{-i\phi}\sin(\theta/2),\cos(\theta/2))^{\mathsf T}$ obeys $(\boldsymbol\sigma\cdot\mathbf n)\chi_-=-\chi_-$ and supplies the other branch at $+k\mathbf n$.

The [Pauli matrix multiplication law](../../../../pauli-matrix-multiplication-law.md) independently gives $H(\mathbf k)^2=(\hbar v)^2|\mathbf k|^2I$. The [dispersion relation](../../../../dispersion-relation-split.md) is therefore a pair of cones touching at zero [energy](../../../../energy-split.md) and [momentum](../../../../momentum-split.md); a signed straight-line cut has upper and lower branches $\pm\hbar v|k_x|$. In the $k_z=0$ plane, $\theta=\pi/2$, and the upper-branch mean [spin](../../../../spin.md) points radially outwards, the lower-branch [spin](../../../../spin.md) radially inwards. This is [spin-momentum locking](../../../../spin-momentum-locking.md), not a tangential [spin](../../../../spin.md) texture. At the touching point the two states are degenerate and the [spin](../../../../spin.md) direction is not selected by the [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md).

<a id="section-b/b3/image-radial-spin-locking-and-a-shifted-weyl-cone-including-a-plane-that-misses-its-node"></a>
![](../../../../past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2018-weyl-dispersion.png)

**[Figure 3](#section-b/b3/image-radial-spin-locking-and-a-shifted-weyl-cone-including-a-plane-that-misses-its-node). Radial spin locking and a shifted Weyl cone, including a plane that misses its node**.

Now let a spatially constant perturbation have [matrix](../../../../matrix.md) $V=\begin{pmatrix}u&w\\w^*&z\end{pmatrix}$, with $u,z$ real. The [Hermitian two-by-two matrix in the Pauli basis](../../../../hermitian-two-by-two-matrix-in-the-pauli-basis.md) decomposition follows explicitly from

$$
\begin{pmatrix}u&w\\w^*&z\end{pmatrix}=dI+a\sigma_x+b\sigma_y+c\sigma_z=\begin{pmatrix}d+c&a-ib\\a+ib&d-c\end{pmatrix},
$$

where $d=(u+z)/2$, $c=(u-z)/2$, $a=\operatorname{Re}w$, and $b=-\operatorname{Im}w$ are real. Equivalently, $d=\operatorname{tr}V/2$ and $(a,b,c)_i=\operatorname{tr}(V\sigma_i)/2$. The four [matrices](../../../../matrix.md) are [linearly independent](../../../../linear-independence.md) under the [trace](../../../../matrix-trace.md) [inner product](../../../../inner-product-split.md) and span the four-dimensional [real vector space](../../../../real-vector-space.md) of Hermitian two-by-two [matrices](../../../../matrix.md).

Spatial constancy means the perturbation does not mix different [wavevectors](../../../../wavevector.md), so each [momentum](../../../../momentum-split.md) sector can still be diagonalized independently. Write $\mathbf b=(a,b,c)$. The full [matrix](../../../../matrix.md) and its exact [eigenvalues](../../../../eigenvalue.md) are

$$
H'(\mathbf k)=dI+(\hbar v\mathbf k+\mathbf b)\cdot\boldsymbol\sigma,\qquad \boxed{E_\pm(\mathbf k)=d\pm\sqrt{(\hbar vk_x+a)^2+(\hbar vk_y+b)^2+(\hbar vk_z+c)^2}.}
$$

This [constant matrix perturbation of a Weyl Hamiltonian](../../../../constant-matrix-perturbation-of-a-weyl-hamiltonian.md) translates the cone to

$$
\boxed{\mathbf k_*=-\frac{(a,b,c)}{\hbar v},\qquad E_*=d.}
$$

In three-dimensional [momentum space](../../../../momentum-space.md) the [energy bands](../../../../energy-band.md) still touch; the perturbation produces no full [spectral gap](../../../../spectral-gap.md). The new branch [spin](../../../../spin.md) directions are parallel and antiparallel to $\hbar v\mathbf k+\mathbf b$, so their radial texture is centered on the shifted point.

A restricted cut must be distinguished from the full [dispersion relation](../../../../dispersion-relation-split.md). In the fixed plane $k_z=0$, the energies are $d\pm\sqrt{(\hbar vk_x+a)^2+(\hbar vk_y+b)^2+c^2}$, with minimum branch separation $2|c|$. This plane misses the crossing if $c\ne0$. Along any line through $\mathbf k_*$ the [dispersion relation](../../../../dispersion-relation-split.md) still crosses linearly. Thus a sketch of a gapped fixed-plane cut alone would not describe the gapless three-dimensional [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md). The cone after a general perturbation is also no longer a function of $|\mathbf k|$ about the old origin alone.

## ↑ Ancestors (13)

1. [B3](../b3.md)
2. [Section B](../../section-b.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../split.md)
5. [Advanced Quantum Physics course of the University of Cambridge](../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
