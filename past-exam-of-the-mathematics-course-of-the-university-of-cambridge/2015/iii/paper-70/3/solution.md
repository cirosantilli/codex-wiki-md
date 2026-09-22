<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Fix the convention $\Delta q-m^2q=0$, $m>0$, and let $c_m=m^2/4$. With $z=x+iy$, two families of [modified Helmholtz adjoint plane waves](../../../../../modified-helmholtz-adjoint-plane-wave.md) are

$$
E_+(z,k)=e^{-ikz+ic_m\bar z/k},\qquad E_-(z,k)=e^{ik\bar z-ic_mz/k},\qquad k\ne0.
$$

Both satisfy $\Delta E_\pm=m^2E_\pm$, since the products of their $z$ and $\bar z$ exponents are $m^2/4$. They obey $E_-(z,k)=\overline{E_+(z,\bar k)}$. [Green second identity](../../../../../green-second-identity.md) gives the two [conjugate global relations for the modified Helmholtz equation](../../../../../conjugate-global-relations-for-the-modified-helmholtz-equation.md)

$$
\boxed{\mathcal G_\pm(k)=\int_{\partial\Omega}\left(E_\pm\partial_nq-q\partial_nE_\pm\right)ds=0.}
$$

For real boundary traces, $\mathcal G_-(k)=\overline{\mathcal G_+(\bar k)}$. Thus the second identity is the conjugate spectral companion, rather than an unrelated extra boundary condition. In complex differential form the first relation is equivalently

$$
\int_{\partial\Omega}E_+\left[(q_z+ikq)dz-\left(q_{\bar z}-\frac{ic_m}{k}q\right)d\bar z\right]=0.
$$

Its integrand is a closed one-form: differentiating its coefficients gives $2E_+(q_{z\bar z}-c_mq)=0$. This supplies a direct derivation of the [global relation](../../../../../global-relation-for-a-linear-boundary-value-problem.md) as well as its outward-normal sign convention.

Write the known [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) on side $j$ as $f_j(s)$ and the unknown outward [normal derivative](../../../../../normal-derivative.md) as $h_j(s)$, with $-1<s<1$. For any linear combination $v$ of the adjoint waves, the [global relation](../../../../../global-relation-for-a-linear-boundary-value-problem.md) is

$$
\sum_j\int_{-1}^1v_j(s)h_j(s)ds=\sum_j\int_{-1}^1f_j(s)\partial_{n_j}v_j(s)ds.
$$

Expanding the $h_j$ in a finite basis and enforcing these identities at selected [collocation points for a global relation](../../../../../collocation-points-for-a-global-relation.md) gives a linear system with a known right side. The square permits especially simple paired tests.

Let $p_n=n\pi/2$, $\eta_n=\sqrt{m^2+p_n^2}$, and $\varphi_n(s)=\sin[p_n(s+1)]$ for $n\geq1$. Define four real adjoint solutions

$$
\begin{aligned}
v_{B,n}&=e^{-\eta_n(y+1)}\varphi_n(x),&v_{T,n}&=e^{\eta_n(y-1)}\varphi_n(x),\\
v_{L,n}&=e^{-\eta_n(x+1)}\varphi_n(y),&v_{R,n}&=e^{\eta_n(x-1)}\varphi_n(y).
\end{aligned}
$$

They satisfy the [modified Helmholtz equation](../../../../../modified-helmholtz-equation.md) because $\eta_n^2-p_n^2=m^2$. Each is a linear combination of two adjoint exponentials, hence is obtained from the two spectral [global relations](../../../../../global-relation-for-a-linear-boundary-value-problem.md). More explicitly, put $\rho_n^\pm=(\eta_n\pm p_n)/2$, so $\rho_n^+\rho_n^-=c_m$. For the $E_+$ convention above, the required spectral pairs are

$$
\boxed{\{\rho_n^+,\rho_n^-\}\ (T),\quad\{-\rho_n^+,-\rho_n^-\}\ (B),\quad\{i\rho_n^+,i\rho_n^-\}\ (R),\quad\{-i\rho_n^+,-i\rho_n^-\}\ (L).}
$$

Appropriate phase-weighted differences produce $\sin[p_n(s+1)]$. For example the top test is $e^{-\eta_n}[e^{ip_n}E_+(\rho_n^-)-e^{-ip_n}E_+(\rho_n^+)]/(2i)$. The conjugate relation ensures a real system for real data. This is [sine collocation of square modified Helmholtz global relations](../../../../../sine-collocation-of-square-modified-helmholtz-global-relations.md).

The functions $\varphi_n$ are an orthonormal [Fourier sine basis](../../../../../fourier-sine-basis.md) on $[-1,1]$. Set $h_{j,n}=\int_{-1}^1h_j\varphi_n ds$ and compute the known quantity $R_{j,n}=\int_{\partial\Omega}f\partial_nv_{j,n}ds$ by numerical integration. Since $\varphi_n(\pm1)=0$, each adjoint test vanishes on both adjacent sides. On its own side it equals $\varphi_n$, and on the opposite side it equals $\delta_n\varphi_n$, where $\delta_n=e^{-2\eta_n}$. Thus the [square modified Helmholtz Dirichlet-to-Neumann coefficients](../../../../../square-modified-helmholtz-dirichlet-to-neumann-coefficients.md) obey

$$
\begin{pmatrix}1&\delta_n\\\delta_n&1\end{pmatrix}\begin{pmatrix}h_{B,n}\\h_{T,n}\end{pmatrix}=\begin{pmatrix}R_{B,n}\\R_{T,n}\end{pmatrix},\qquad
\begin{pmatrix}1&\delta_n\\\delta_n&1\end{pmatrix}\begin{pmatrix}h_{L,n}\\h_{R,n}\end{pmatrix}=\begin{pmatrix}R_{L,n}\\R_{R,n}\end{pmatrix}.
$$

Each block is inverted explicitly: for opposite sides $j,j'$,

$$
\boxed{h_{j,n}=\frac{R_{j,n}-\delta_nR_{j',n}}{1-\delta_n^2}.}
$$

Compute these coefficients for $1\leq n\leq N$ and reconstruct $h_j^{(N)}=\sum_{n=1}^Nh_{j,n}\varphi_n$. This is a semi-analytical scheme: the spectral basis integrals and two-by-two inverses are explicit, while the known boundary integrals are evaluated numerically. Increase $N$ and the quadrature resolution until the desired convergence is observed; compatible smooth side data have convergent normal-trace expansions, while corner singularities require the usual weaker trace interpretation and more careful quadrature.

The requested weak interaction between sides is particularly clear: **the adjacent-side unknown traces contribute exactly zero, and the opposite-side coefficient is $e^{-2\sqrt{m^2+(n\pi/2)^2}}\to0$**. The own-side coefficient stays equal to one. Thus [diagonal dominance of paired square global-relation collocation](../../../../../diagonal-dominance-of-paired-square-global-relation-collocation.md) is genuine after pairing; individual uncombined exponential samples need not have the same conditioning. The eigenvalues of each block are $1\pm\delta_n$, so its condition number is $(1+\delta_n)/(1-\delta_n)$.

There is also a direct localization check for an individual adjoint wave. On side $j$ with outward unit normal $n_j$ and tangent $t_j$, the normalized test $e^{\eta(n_j\cdot r-1)+ip\,t_j\cdot r}$ has $\eta=\sqrt{m^2+p^2}$. Its opposite-side magnitude is $e^{-2\eta}$, and its magnitude integrates to at most $1/\eta$ along either adjacent side. This [side localization of modified Helmholtz plane waves](../../../../../side-localization-of-modified-helmholtz-plane-waves.md) explains why suitable large spectral parameters suppress remote-side effects even before the exact sine cancellation.

Finally the interior solution can be evaluated from the computed traces using the [two-dimensional modified Helmholtz fundamental solution](../../../../../two-dimensional-modified-helmholtz-fundamental-solution.md)

$$
\Gamma_m(r,s)=\frac1{2\pi}K_0(m|r-s|),\qquad q(r)=\int_{\partial\Omega}\left[\Gamma_m(r,s)h(s)-f(s)\partial_{n_s}\Gamma_m(r,s)\right]ds.
$$

Here $K_0$ is the [Modified Bessel function of the second kind](../../../../../modified-bessel-function-of-the-second-kind.md), and $(-\Delta+m^2)\Gamma_m=\delta$. Replace $h$ by its computed finite [Fourier sine series](../../../../../fourier-sine-series.md) and use numerical integration; at interior points the boundary kernels are smooth. The sign follows from [Green second identity](../../../../../green-second-identity.md) with this fundamental-solution convention. This completes the numerical integration of the [boundary value problem](../../../../../boundary-value-problem.md) with a [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md), rather than stopping at an equation for its unknown boundary derivatives.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
