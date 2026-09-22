<h1 id="33b/solution">Solution</h1>

↑ **Parent:** [33B](../33b.md)

Translate the scattering solution for the atom at the origin by $\mathbf a$. Its incident wave becomes $e^{i\mathbf k\cdot(\mathbf r-\mathbf a)}$; multiplying the whole solution by $e^{i\mathbf k\cdot\mathbf a}$ restores the prescribed incident wave. At large $r$,

$$
|\mathbf r-\mathbf a|=r-\widehat{\mathbf r}\cdot\mathbf a+O(r^{-1}),
\qquad\widehat{\mathbf r-\mathbf a}=\widehat{\mathbf r}+O(r^{-1}).
$$

Thus the outgoing amplitude acquires the phase $e^{i(\mathbf k-\mathbf k')\cdot\mathbf a}$, with $\mathbf k'=k\widehat{\mathbf r}$.

In the single-scattering approximation, amplitudes from lattice sites add coherently. If $\mathbf Q=\mathbf k-\mathbf k'$,

$$
\frac{d\sigma}{d\Omega}=|f(\widehat{\mathbf r})|^2
\left|\sum_{\mathbf a\in\mathcal L_N}e^{i\mathbf Q\cdot\mathbf a}\right|^2,
\qquad
\boxed{\Delta(\mathbf Q)=\frac1N
\left|\sum_{\mathbf a\in\mathcal L_N}e^{i\mathbf Q\cdot\mathbf a}\right|^2.}
$$

For a rectangular block of a [Bravais lattice](../../../../../bravais-lattice.md) with $N_j$ sites along primitive vectors $\mathbf a_j$ and $N=N_1N_2N_3$, the [geometric series](../../../../../geometric-series.md) gives

$$
\boxed{\Delta(\mathbf Q)=\frac1N
\prod_{j=1}^3
\left[\frac{\sin(N_j\mathbf Q\cdot\mathbf a_j/2)}
{\sin(\mathbf Q\cdot\mathbf a_j/2)}\right]^2.}
$$

Each ratio has its limiting value $N_j$ when its argument is a multiple of $2\pi$. Thus the peaks have height $N$ and widths of order $1/N_j$ in those phase variables, at $\mathbf Q\cdot\mathbf a_j\in2\pi\mathbb Z$, exactly the [reciprocal lattice](../../../../../reciprocal-lattice.md) vectors.

With the incident-wave normalization used here, the [Born approximation](../../../../../born-approximation.md) is

$$
f_B(\widehat{\mathbf r})=-\frac{m_e}{2\pi\hbar^2}
\int_{\mathbb R^3}e^{i(\mathbf k-\mathbf k')\cdot\mathbf r}
V(\mathbf r)\,d^3r.
$$

For the stated attractive three-dimensional delta potential,

$$
\boxed{f_B=\frac{m_ea}{2\pi\hbar^2},}
$$

independent of scattering angle. This is the formal first Born amplitude, not a claim that an unregularized three-dimensional delta interaction defines an exact scattering Hamiltonian.

The 60-degree scattering angle is twice the Bragg angle, so $\theta=30^\circ$. First-order [elastic Bragg scattering condition](../../../../../elastic-bragg-scattering-condition.md) gives $2d\sin\theta=\lambda$, hence

$$
\boxed{d=\lambda.}
$$

Higher orders would give $d=n\lambda$; the smallest, usual first-order spacing is the likely answer.

## ↑ Ancestors (10)

1. [33B](../33b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
