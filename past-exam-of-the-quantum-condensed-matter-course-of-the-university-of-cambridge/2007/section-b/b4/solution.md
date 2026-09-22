<h1 id="section-b/b4/solution">Solution</h1>

↑ **Parent:** [B4](../b4.md)

[Bloch's theorem](../../../../bloch-s-theorem-split.md) states that an eigenfunction in a periodic potential can be written $\psi_{\mathbf k}(\mathbf r)=e^{i\mathbf k\cdot\mathbf r}u_{\mathbf k}(\mathbf r)$, with $u_{\mathbf k}$ lattice-periodic. In the [orthogonal tight-binding approximation](../../../../orthogonal-tight-binding-approximation.md), choose localized orthonormal orbitals $|j\rangle$ with on-site matrix element $E_0$ and real nearest-neighbour [hopping integral](../../../../hopping-integral.md) $t$. The Bloch sum $|k\rangle=N^{-1/2}\sum_j e^{ikja}|j\rangle$ is an eigenstate because each neighbour shift contributes a phase $e^{\pm ika}$. Thus

$$
\boxed{E(k)=E_0+t(e^{ika}+e^{-ika})=E_0+2t\cos ka.}
$$

The [simple-cubic nearest-neighbour tight-binding band](../../../../simple-cubic-nearest-neighbour-tight-binding-band.md) has six neighbours, giving $E(\mathbf k)=E_0+2t[\cos(k_xa)+\cos(k_ya)+\cos(k_za)]$. The cosine sum ranges from $-3$ to $3$, so the positive [bandwidth](../../../../bandwidth-signal-processing.md) is $W=12|t|$. The stated hopping formula is negative when $E_1>0$, so the printed $12t$ must be read as a bandwidth magnitude.

Near the zone centre, $E=E_0+6t-ta^2k^2+O(k^4)$. To leading order the constant-energy surfaces are spheres, and comparison with $E_\Gamma+\hbar^2k^2/(2m^*)$ gives

$$
\boxed{m^*=-\frac{\hbar^2}{2ta^2}=\frac{\hbar^2e^{a/a_1}}{4E_1a^2(1+a/a_1)}.}
$$

This is the [effective mass for overlap-weighted exponential hopping](../../../../effective-mass-for-overlap-weighted-exponential-hopping.md). With $s=a/a_1$, its logarithmic derivative is $d\ln m^*/ds=1-2/s-1/(1+s)$. The positive stationary point is $s=1+\sqrt3$, and it is a minimum. The formula grows at both very small and very large $s$; the small-separation divergence is a mathematical extrapolation into a regime where localized tight binding itself becomes unreliable.

<a id="section-b/b4/image-competing-orbital-hopping-and-geometric-curvature-give-an-effective-mass-minimum"></a>
![](../../../../past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2007-tight-binding-mass.png)

**[Figure 4](#section-b/b4/image-competing-orbital-hopping-and-geometric-curvature-give-an-effective-mass-minimum). Competing orbital hopping and geometric curvature give an effective-mass minimum**. The mass is plotted in units $\hbar^2/(4E_1a_1^2)$ against $a/a_1$. The marked minimum is at $1+\sqrt3$; the formula's small-spacing continuation should not be treated as a quantitative strong-overlap model.

For the bandwidth, $W=24E_1(1+s)e^{-s}$ and $d\ln W/d\ln a=-s^2/(1+s)$. At $s=1$, a fractional spacing change $-0.01$ therefore gives

$$
\boxed{\frac{\Delta W}{W}\simeq+0.005=+0.50\%.}
$$

The exact ratio $W(0.99a_1)/W(a_1)=(1.99/2)e^{0.01}=1.004999916\ldots$ checks the first-order result. Compression strengthens the hopping and widens the band.

## ↑ Ancestors (13)

1. [B4](../b4.md)
2. [Section B](../../section-b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../split.md)
5. [Quantum Condensed Matter course of the University of Cambridge](../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
