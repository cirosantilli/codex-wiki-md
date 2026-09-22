<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $R_j$ for the rectangles, $x_j$ for their centers and $e_j$ for their long-axis directions. For the finite exponent $p$ in the displayed estimate, take smooth rotated cap functions $\psi_j$, with $0\le\psi_j\le1$, equal to one on angular distance at most $\delta/C$ from $e_j$ and supported within $2\delta/C$. Choose $C$ sufficiently large once and for all. The direction separation makes these cap supports disjoint, and $\int|\psi_j|^p\,d\sigma\lesssim\delta$.

Define

$$
f_j(\omega)=e^{ix_j\cdot\omega}\psi_j(\omega),\qquad
h_j(x)=\widehat{f_j\,d\sigma}(x)
=\widehat{\psi_j\,d\sigma}(x-x_j).
$$

The [Fourier modulation and translation identity](../../../../../../modulation-property-of-the-fourier-transform.md) gives the second equality. Rotating the [circle cap Fourier lower bound](../../../../../../circle-cap-fourier-lower-bound.md) then gives **$|h_j(x)|\gtrsim\delta$ on $R_j$**. The half-side lengths of $R_j$ are no larger than the two frequency bounds used in part (b).

Let $\varepsilon_j$ be independent [Rademacher random variables](../../../../../../rademacher-distribution.md). Because the input cap supports are disjoint, for every choice of signs

$$
\left\|\sum_j\varepsilon_j f_j\right\|_{L^p(\sigma)}^p
=\sum_j\|\psi_j\|_{L^p(\sigma)}^p\lesssim M\delta,
$$

where $M=\#\mathcal R$. Apply the assumed [Fourier extension estimate](../../../../../../fourier-extension-estimate.md) to the sum. Average over signs and use the [Khintchine inequality](../../../../../../khintchine-inequality.md) pointwise, followed by the [Tonelli theorem](../../../../../../tonelli-theorem.md):

$$
\int_{\mathbb R^2}\left(\sum_j|h_j(x)|^2\right)^{p/2}\,dx
\lesssim_p\mathbb E\left\|\sum_j\varepsilon_jh_j\right\|_p^p
\lesssim_p M\delta.
$$

There is no requirement that the spatial rectangles be disjoint; disjointness is used only for the input caps on the [unit circle](../../../../../../complex-unit-circle.md). Their spatial overlaps are precisely what the square function measures. The cap lower bounds now imply

$$
\delta^p\int\left(\sum_j\mathbf1_{R_j}\right)^{p/2}
\lesssim_p M\delta.
$$

Since each rectangle has area $\delta^{-3}$, the [restriction-to-rectangle overlap principle](../../../../../../restriction-to-rectangle-overlap-principle.md) gives

$$
\boxed{\int\left(\sum_{R\in\mathcal R}\mathbf1_R\right)^{p/2}
\lesssim_p M\delta^{1-p}
=\delta^{4-p}\sum_{R\in\mathcal R}|R|.}
$$

The constants are independent of $\delta$, the centers and the collection. The finite-$p$ interpretation is the one for which the printed power integral is defined. A single cap also shows that the assumed diagonal [Fourier extension estimate](../../../../../../fourier-extension-estimate.md) can hold only for $p\ge4$: its output contributes at least $\delta^{p-3}$ to the $p$th-power [norm](../../../../../../norm.md), whereas its input contributes at most a constant times $\delta$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
