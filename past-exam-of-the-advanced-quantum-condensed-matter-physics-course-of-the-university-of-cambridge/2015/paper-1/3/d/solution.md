<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use $|j\rangle$ for the six printed basis vectors. The three singly occupied triplets are

$$
|T_+\rangle=|1\rangle,\qquad
|T_0\rangle=\frac{|2\rangle+|3\rangle}{\sqrt2},\qquad
|T_-\rangle=|4\rangle.
$$

Each has **[energy](../../../../../energy-split.md) zero**: either Pauli exclusion prevents hopping to [double occupancy](../../../../../double-occupancy.md) or the two contributions cancel. Define

$$
|S\rangle=\frac{|2\rangle-|3\rangle}{\sqrt2},\quad
|D_+\rangle=\frac{|5\rangle+|6\rangle}{\sqrt2},\quad
|D_-\rangle=\frac{|5\rangle-|6\rangle}{\sqrt2}.
$$

The state $D_-$ has [energy](../../../../../energy-split.md) $U$. In the $S,D_+$ subspace the [Hamiltonian](../../../../../hamiltonian.md) is $\bigl(\begin{smallmatrix}0&-2t\\-2t&U\end{smallmatrix}\bigr)$, with

$$
E_\pm=\frac{U\pm\sqrt{U^2+16t^2}}2.
$$

For $U\gg|t|>0$, the fourth low-energy eigenstate is the normalized singlet

$$
\boxed{|\psi_-\rangle=\mathcal N\left(|S\rangle-\frac{E_-}{2t}|D_+\rangle\right)
\simeq\mathcal N\left(|S\rangle+\frac{2t}{U}|D_+\rangle\right),}
$$

where $\mathcal N=[1+(E_-/(2t))^2]^{-1/2}$. Its [energy](../../../../../energy-split.md) is

$$
\boxed{E_-=-\frac{4t^2}{U}+O(t^4/U^3).}
$$

The **four lowest energies are $-4t^2/U,0,0,0$ to leading order**, with the singlet and triplets just given. The upper pair lie near $U$ and $U+4t^2/U$.

The low-energy [Hamiltonian](../../../../../hamiltonian.md) can be written

$$
\boxed{H_{\rm eff}=J\left(\mathbf S_1\cdot\mathbf S_2-\frac14\right),\qquad
J=\frac{4t^2}{U}>0,}
$$

using dimensionless spin-half operators. It places the singlet below the triplet by $J$, hence favors antiferromagnetic alignment. A [lattice](../../../../../lattice.md) of such bonds can support [antiferromagnetism](../../../../../antiferromagnetism.md), although its ordering pattern also depends on geometry and competing couplings. The physical [energy](../../../../../energy-split.md) gain comes from virtual charge fluctuations, not from a permanent [double occupancy](../../../../../double-occupancy.md) in the large-$U$ limit.

<a id="3/d/image-exact-singlet-triplet-spectrum-of-the-two-site-repulsive-hubbard-model-and-the-large-u-exchange-scale"></a>
![](../../../../../past-exam-of-the-advanced-quantum-condensed-matter-physics-course-of-the-university-of-cambridge/2015/paper-1-hubbard-spectrum.png)

**[Figure 4](#3/d/image-exact-singlet-triplet-spectrum-of-the-two-site-repulsive-hubbard-model-and-the-large-u-exchange-scale). Exact singlet-triplet spectrum of the two-site repulsive Hubbard model and the large-U exchange scale**.

## ↑ Ancestors (14)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the advanced Quantum Condensed Matter Physics course of the University of Cambridge](../../../../split.md)
6. [Advanced Quantum Condensed Matter Physics course of the University of Cambridge](../../../../../advanced-quantum-condensed-matter-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
