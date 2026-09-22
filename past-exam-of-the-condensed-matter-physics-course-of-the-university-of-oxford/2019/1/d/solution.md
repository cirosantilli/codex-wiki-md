<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Separate the entire-system atom index into a cell translation $\mathbf R$ and an index $p$ within a single [primitive unit cell](../../../../primitive-unit-cell.md). The potential becomes

$$
V(\mathbf x)=\sum_{\mathbf R\ \mathrm{all\ cells}}\sum_{p\ \mathrm{one\ cell}}u_p(\mathbf x-\mathbf R-\mathbf r_p).
$$

The same $u_p$ is used in every translated cell because the [atomic basis](../../../../atomic-basis-of-a-crystal.md) repeats. Normalize [plane waves](../../../../plane-wave.md) in volume $\Omega$ by $\langle\mathbf x|\mathbf k\rangle=\Omega^{-1/2}e^{i\mathbf k\cdot\mathbf x}$. For $\mathbf G=\mathbf k'-\mathbf k$, substitution and $\mathbf s=\mathbf x-\mathbf R-\mathbf r_p$ give

$$
\langle\mathbf k'|V|\mathbf k\rangle=\frac1\Omega\left[\sum_{\mathbf R\ \mathrm{all\ cells}}e^{-i\mathbf G\cdot\mathbf R}\right]\left[\sum_{p\ \mathrm{one\ cell}}e^{-i\mathbf G\cdot\mathbf r_p}\int d^3s\,e^{-i\mathbf G\cdot\mathbf s}u_p(\mathbf s)\right].
$$

For a real static scalar potential, define the [atomic scattering factor](../../../../atomic-scattering-factor.md) in the positive-exponent convention of the question by

$$
\boxed{b_p(\mathbf G)=\int d^3s\,e^{i\mathbf G\cdot\mathbf s}u_p(\mathbf s),\qquad S(\mathbf G)=\sum_{p\ \mathrm{one\ cell}}b_p(\mathbf G)e^{i\mathbf G\cdot\mathbf r_p}.}
$$

The second bracket in the matrix element is $S(\mathbf G)^*$. At a [reciprocal lattice vector](../../../../reciprocal-lattice-vector.md) every term of the first bracket is one, giving the number of cells $N_c$. Therefore the stated transition-rate rule, equivalently the first [Born approximation](../../../../born-approximation.md) and [Fermi's golden rule](../../../../fermi-s-golden-rule.md) up to the final-state kinematic factors, yields

$$
\boxed{I(\mathbf G)\propto|\langle\mathbf k'|V|\mathbf k\rangle|^2=\frac{N_c^2}{\Omega^2}|S(\mathbf G)|^2\propto|S(\mathbf G)|^2.}
$$

The harmless complex conjugation records the distinction between the source's positive-exponent [Fourier transform](../../../../fourier-transform-split.md) and the usual positive-exponent incoming [plane wave](../../../../plane-wave.md). Reversing every Fourier sign gives the equivalent amplitude convention. Only the cell-translation sum ranges over the full crystal; the [crystal basis structure factor](../../../../crystal-basis-structure-factor.md) contains the atoms of one cell.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
