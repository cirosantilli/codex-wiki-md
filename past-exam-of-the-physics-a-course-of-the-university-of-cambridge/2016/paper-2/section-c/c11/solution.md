<h1 id="section-c/c11/solution">Solution</h1>

↑ **Parent:** [C11](../c11.md)

The [reciprocal lattice](../../../../../reciprocal-lattice.md) consists of all [wavevectors](../../../../../wavevector.md) $\mathbf G$ whose plane-wave phase is unchanged under every direct-lattice translation $\mathbf R$:

$$
e^{i\mathbf G\cdot\mathbf R}=1,\qquad
\mathbf G\cdot\mathbf R\in2\pi\mathbb Z.
$$

It expresses periodicity in [wavevector](../../../../../wavevector.md) space, with dimensions of inverse length.

Choose incident field convention $e^{i\mathbf k_i\cdot\mathbf r-i\omega t}$. The [wave](../../../../../wave-split.md) at the second atom acquires incident phase $\mathbf k_i\cdot\mathbf r_n$ relative to the atom at the origin. Its path to a distant detector is shorter by approximately $\hat{\mathbf k}_f\cdot\mathbf r_n$, contributing outgoing phase $-\mathbf k_f\cdot\mathbf r_n$. Therefore

$$
\Delta\phi=(\mathbf k_i-\mathbf k_f)\cdot\mathbf r_n
=\mathbf k_s\cdot\mathbf r_n.
$$

Neglecting variation of detector distance across the specimen, identical atoms have a common scattering amplitude factor and

$$
\boxed{S\propto\sum_ne^{i\mathbf k_s\cdot\mathbf r_n}.}
$$

The original geometry diagram shows the incident direction, outgoing direction and direct-space [displacement](../../../../../displacement.md) separately; $\mathbf k_s$ is a [wavevector](../../../../../wavevector.md) difference, not an extra ray path.

The primitive reciprocal vectors obey

$$
\boxed{\mathbf A\cdot\mathbf a=2\pi,\qquad
\mathbf A\cdot\mathbf b=\mathbf A\cdot\mathbf c=0,}
$$

with cyclic versions for $\mathbf B,\mathbf C$. If $\mathbf k_s=h\mathbf A+k\mathbf B+l\mathbf C$, every [lattice](../../../../../lattice.md) term has phase $2\pi$ times an integer, so all terms add constructively. Conversely, full translational reinforcement requires $\mathbf k_s\cdot\mathbf a$, $\mathbf k_s\cdot\mathbf b$ and $\mathbf k_s\cdot\mathbf c$ to be integer multiples of $2\pi$, hence $\mathbf k_s$ is reciprocal. These are the [Laue equations](../../../../../laue-equations.md). A finite [crystal](../../../../../crystal.md) gives finite-width maxima rather than ideal reciprocal-space delta peaks; elastic scattering must also satisfy $|\mathbf k_i|=|\mathbf k_f|$.

For the two-dimensional [Bravais lattice](../../../../../bravais-lattice.md) interpretation, with one atom per primitive cell, take

$$
\mathbf a=a(1,0),\qquad
\mathbf b=a(1/2,\sqrt3/2).
$$

Solving the duality conditions gives

$$
\mathbf A=\frac{2\pi}{a}(1,-1/\sqrt3),\qquad
\mathbf B=\frac{2\pi}{a}(0,2/\sqrt3),
$$

so

$$
\boxed{\mathbf G_{hk}=\frac{2\pi}{a}
\left(h,\frac{2k-h}{\sqrt3}\right),\qquad
|\mathbf G_{hk}|^2=\frac{16\pi^2}{3a^2}(h^2-hk+k^2).}
$$

The reciprocal primitive vectors have equal length $4\pi/(\sqrt3a)$ and angle $120^\circ$; the array itself is triangular. A different primitive basis can use a $60^\circ$ angle without changing the [lattice](../../../../../lattice.md). The direct primitive-cell area is $\sqrt3a^2/2$ and its reciprocal-cell area is $(2\pi)^2$ divided by that area.

For nonzero integer pairs, $h^2-hk+k^2$ has minimum one, attained for six shortest vectors. Therefore **the first nonforward maximum has $|\mathbf k_s|=4\pi/(\sqrt3a)$**. If the forward transmitted maximum is included literally, the smallest value is **$|\mathbf k_s|=0$**; the nonzero value is the first [diffraction](../../../../../diffraction.md) shell. Reaching that shell in elastic scattering additionally requires $4\pi/(\sqrt3a)\leq2|\mathbf k_i|$.

## ↑ Ancestors (14)

1. [C11](../c11.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2016](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
