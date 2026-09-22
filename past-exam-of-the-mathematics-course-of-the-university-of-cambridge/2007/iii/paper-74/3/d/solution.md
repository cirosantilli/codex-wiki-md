<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

By symmetry the normalized [covariance matrix](../../../../../../covariance-matrix.md) has the form $\eta=\begin{pmatrix}V&W\\W&V\end{pmatrix}$. Substituting the matrices from part (c) into the [normalized stationary fluctuation-dissipation relation for a reaction network](../../../../../../normalized-stationary-fluctuation-dissipation-relation-for-a-reaction-network.md), $M\eta+\eta M^{\mathsf T}=D$, gives

$$
\frac2\tau\begin{pmatrix}V+EW&W+EV\\W+EV&V+EW\end{pmatrix}
=\frac1{\tau\mu}\begin{pmatrix}2&E\\E&2\end{pmatrix}.
$$

Hence $V+EW=1/\mu$ and $W+EV=E/(2\mu)$. Solving these two equations gives the [linear noise of two species with joint removal](../../../../../../linear-noise-of-two-species-with-joint-removal.md):

$$
\boxed{V=\frac{2-E^2}{2\mu(1-E^2)},\qquad
W=-\frac{E}{2\mu(1-E^2)},\qquad
\eta=\frac1{2\mu(1-E^2)}\begin{pmatrix}2-E^2&-E\\-E&2-E^2\end{pmatrix}.}
$$

For $E=0$ the normalized variance is $1/\mu$ and the covariance is zero, as expected for independent immigration–death processes. For $E>0$, $V=1/\mu+E^2/(2\mu(1-E^2))$ exceeds this independent value and $W<0$. The [correlation coefficient](../../../../../../pearson-correlation-coefficient.md) is

$$
\rho=\frac WV=-\frac{E}{2-E^2}\longrightarrow-1\quad(E\to1).
$$

This negative stationary correlation is compatible with positive instantaneous joint-removal noise: the slow difference mode amplifies fluctuations of opposite signs in the two populations.

The symmetric and antisymmetric [eigenvectors](../../../../../../eigenvector.md) diagonalize all three matrices. Their normalized covariance eigenvalues are

$$
\eta_+=V+W=\frac{2+E}{2\mu(1+E)},\qquad
\eta_-=V-W=\frac{2-E}{2\mu(1-E)}.
$$

The corresponding restoring rates are $(1+E)/\tau=\beta+2C\mu$ and $(1-E)/\tau=\beta$. Thus the sum mode retains finite fluctuations, with $\eta_+\to3/(4\mu)$, whereas the difference mode becomes arbitrarily noisy. In particular, at a fixed nonzero mean, or along $\beta\to0$ at fixed $\lambda,C>0$ so $\mu\to\sqrt{\lambda/C}$,

$$
\boxed{V\sim\frac1{4\mu(1-E)}\to+\infty,\qquad
W\sim-\frac1{4\mu(1-E)}\to-\infty.}
$$

The [Fano factor](../../../../../../fano-factor.md) of either population is $\mu V=(2-E^2)/(2(1-E^2))$, which diverges as $E\to1$ regardless of how the mean is varied. Unnormalized variances are $\mu^2V$ and covariance $\mu^2W$, so their absolute magnitudes also depend on the parameter path through $\mu$.

The [phase plane](../../../../../../phase-plane.md) in part (b) explains the singularity. At $\beta=0$, the mean-field system has a whole hyperbola of equilibria, rather than an isolated restoring state. A perturbation in the species difference selects another point on that curve. In the actual stochastic reaction network, joint complex formation still leaves $X_1-X_2$ unchanged, but the two constant-rate births change it by $+1$ and $-1$, each at rate $\lambda$. Therefore [exclusive joint removal has a diffusing difference mode](../../../../../../exclusive-joint-removal-has-a-diffusing-difference-mode.md):

$$
\operatorname{Var}(X_1(t)-X_2(t))=\operatorname{Var}(X_1(0)-X_2(0))+2\lambda t.
$$

Its [continuous-time symmetric simple random walk](../../../../../../continuous-time-symmetric-simple-random-walk.md) on the integers has no normalizable stationary distribution, so there is **no finite stationary covariance at $E=1$**. The divergence as $E\uparrow1$ signals both the loss of difference-mode restoration and eventual failure of the small-fluctuation [moment closure](../../../../../../moment-closure.md); near the limit, the computed normalized variances need not remain small even when the individual mean populations are large.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
