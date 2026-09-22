<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Here the sphere's “volume” is its intrinsic $(N-1)$-dimensional area, not the volume of the enclosed ball. Write $\Omega_{N-1}$ for the area of the unit sphere. The [Gaussian integral](../../../../../gaussian-integral.md) gives

$$
I_N=\int_{\mathbb R^N}e^{-|x|^2}\,d^Nx=\left(\int_{\mathbb R}e^{-u^2}\,du\right)^N=\pi^{N/2}.
$$

For completeness the one-dimensional integral is positive and its square is $2\pi\int_0^\infty\rho e^{-\rho^2}d\rho=\pi$. In [hyperspherical coordinates](../../../../../hyperspherical-coordinates.md), the same integral is

$$
I_N=\Omega_{N-1}\int_0^\infty\rho^{N-1}e^{-\rho^2}\,d\rho
=\frac{\Omega_{N-1}}2\int_0^\infty u^{N/2-1}e^{-u}\,du
=\frac{\Omega_{N-1}}2\Gamma(N/2).
$$

The substitution is $u=\rho^2$, and the last integral defines the [Gamma function](../../../../../gamma-function.md). Equating the two evaluations and scaling lengths by $r$ proves

$$
\boxed{\Omega_{N-1}=\frac{2\pi^{N/2}}{\Gamma(N/2)},\qquad
V_{N-1}(r)=\frac{2\pi^{N/2}}{\Gamma(N/2)}r^{N-1}.}
$$

Take $D$ to mean spacetime dimension, so the number of spatial dimensions is $d=D-1$. This convention is needed when comparing five-dimensional spacetime with four-dimensional spacetime. For a point charge $q$, [Gauss's law](../../../../../gauss-s-law.md) in $d$ spatial dimensions gives

$$
\Omega_{d-1}r^{d-1}E_r(r)=\frac q{\varepsilon_D}.
$$

Using $E_r=-\phi'(r)$ and choosing $\phi(\infty)=0$ for $d>2$ gives

$$
\boxed{\phi_D(r)=\frac q{\varepsilon_D(d-2)\Omega_{d-1}r^{d-2}}
=\frac{q\,\Gamma((D-1)/2)}{2(D-3)\pi^{(D-1)/2}\varepsilon_D\,r^{D-3}}\quad(D>3).}
$$

The [Green function of the Laplacian](../../../../../green-function-of-the-laplacian.md) with $-\nabla^2G_d=\delta^{(d)}$ is consequently $G_d(r)=1/[(d-2)\Omega_{d-1}r^{d-2}]$. Define the gravitational Poisson coupling $\kappa_D$ by $\nabla^2\Psi=\kappa_DM\delta^{(d)}$, and use acceleration $\mathbf g=-\nabla\Psi$. The same flux calculation gives

$$
\boxed{\Psi_D(r)=-\kappa_DM G_d(r)
=-\frac{\kappa_DM}{(D-3)\Omega_{D-2}r^{D-3}}.}
$$

This explicitly fixes the normalization of the gravitational coupling: in four dimensions $\kappa_4=4\pi G_4$, so $\Psi_4=-G_4M/r$. If a higher-dimensional Newton constant is instead defined by the force law $|\mathbf g|=G_DM/r^{D-2}$, then $\kappa_D=\Omega_{D-2}G_D$ in the displayed expression. In all conventions the force scales as $r^{-(D-2)}$ and the potential as $r^{-(D-3)}$. If “$D$ dimensions” denotes spatial dimensions instead, replace $d$ by $D$ and the potential exponent is $D-2$.

For $d=2$, integration gives $\phi=-q\log(r/r_0)/(2\pi\varepsilon_3)$ and $\Psi=\kappa_3M\log(r/r_0)/(2\pi)$ for the Poisson-normalized gravitational model; these logarithmic potentials have no zero-at-infinity convention. For $d=1$, a fundamental solution of the negative Laplacian is $G_1(x)=-|x|/2$, giving linear potentials up to an additive homogeneous solution.

Now compactify the fourth spatial coordinate $y$ on a circle of circumference $L=2\pi R$, retaining three noncompact coordinates with radial distance $r$. In uncompactified five-dimensional spacetime, $G_4(r,y)=1/[4\pi^2(r^2+y^2)]$. A periodic point source is therefore represented by its images:

$$
G_{\mathrm{circle}}(r,y)=\frac1{4\pi^2}\sum_{n\in\mathbb Z}\frac1{r^2+(y+nL)^2}.
$$

For $r/L\to\infty$, write the sum as $r^{-2}\sum_n[1+(nL/r)^2]^{-1}$ on the source slice $y=0$. The spacing $L/r$ tends to zero, so its Riemann sum approaches the integrable function's integral:

$$
\sum_n\frac1{r^2+n^2L^2}\sim\frac1{Lr}\int_{-\infty}^{\infty}\frac{du}{1+u^2}=\frac\pi{Lr}.
$$

Thus the compactified Green function is asymptotic to $1/(4\pi Lr)$, already proving the four-dimensional inverse-distance law.

An exact expression makes the crossover transparent. The Fourier transform of $(r^2+y^2)^{-1}$ is $\pi e^{-r|k|}/r$, obtained by closing the integration contour around $y=ir$ or $-ir$. Applying the [Poisson summation formula](../../../../../poisson-summation-formula.md) then gives, at $y=0$,

$$
\sum_n\frac1{r^2+n^2L^2}=\frac\pi{Lr}\left(1+2\sum_{n\ge1}e^{-2\pi nr/L}\right)
=\frac\pi{Lr}\coth\left(\frac{\pi r}L\right).
$$

The last equality sums a geometric series. Hence the [point-source potential with one compact spatial dimension](../../../../../point-source-potential-with-one-compact-spatial-dimension.md) is

$$
\boxed{\phi(r,0)=\frac q{4\pi\varepsilon_5Lr}\coth\left(\frac{\pi r}L\right),\qquad
\Psi(r,0)=-\frac{\kappa_5M}{4\pi Lr}\coth\left(\frac{\pi r}L\right).}
$$

At short distances $r\ll L$, $\coth(\pi r/L)\sim L/(\pi r)$ and these reproduce the five-dimensional $1/r^2$ potentials. At long distances $r\gg L$, the hyperbolic factor is $1+O(e^{-2\pi r/L})$, giving the four-dimensional $1/r$ potentials with effective Poisson couplings $\varepsilon_4=L\varepsilon_5$ and $\kappa_4=\kappa_5/L$. Equivalently only the massless [Kaluza-Klein mode](../../../../../kaluza-klein-mode.md) survives at long distance, while the massive modes contribute exponentially suppressed terms.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
