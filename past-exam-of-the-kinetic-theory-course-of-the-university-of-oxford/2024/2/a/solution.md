<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the electron [electric charge](../../../../electric-charge-split.md) $-e$, so $E=-\partial_x\varphi$ gives acceleration $+(e/m_e)\partial_x\varphi$. The [Vlasov equation](../../../../vlasov-equation.md), its average, and its linearized fluctuating part are

$$
\begin{gathered}
\partial_tf+v\partial_xf+\frac e{m_e}\partial_x\varphi\,\partial_vf=0,\\
\partial_tf_0=-\frac e{m_e}\partial_v\langle\partial_x\varphi\,\delta f\rangle,\qquad
(\partial_t+ikv)\delta f_k=-\frac{ike}{m_e}\varphi_k f_0'.
\end{gathered}
$$

The [quasilinear approximation](../../../../quasilinear-approximation.md) retains the averaged quadratic term but drops products of fluctuations from the fluctuating equation. It freezes the slowly evolving $f_0$ during the fast response calculation. A real [electrostatic potential](../../../../electric-potential.md) has $\varphi_{-k}=\varphi_k^*$, and the sum includes both signs of every nonzero [wavenumber](../../../../wavenumber.md). Spatial averaging selects the opposite [Fourier series](../../../../fourier-series-split.md) harmonics; statistical homogeneity supplies the corresponding diagonal noise covariance.

Let $\widehat g(p)=\int_0^\infty e^{-pt}g(t)\,dt$. Zero initial $\delta f_k$ gives

$$
\widehat{\delta f}_k(p,v)=-\frac{ike}{m_e}\frac{f_0'(v)}{p+ikv}\widehat\varphi_k(p).
$$

Insert this into the electrostatic self-consistency relation. Using $\omega_{pe}^2=4\pi e^2n_e/m_e$ and $p+ikv=ik(v-ip/k)$ gives

$$
\epsilon(p,k)\widehat\varphi_k=\widehat\chi_k,\qquad
\epsilon(p,k)=1-\frac{\omega_{pe}^2}{k^2n_e}\int_{C_L}\frac{f_0'(v')}{v'-ip/k}\,dv'.
$$

This derives the stated [dielectric function](../../../../dielectric-function.md) with the [Landau contour](../../../../landau-contour.md). A noise-free growing collective response is a zero of $\epsilon$.

The [Laplace transform](../../../../laplace-transform.md) of the [white noise](../../../../white-noise.md) covariance is particularly simple. Writing $q=p'^*$,

$$
\begin{aligned}
\langle\widehat\chi_k(p)\widehat\chi_k(p')^*\rangle
&=2A_k\int_0^\infty ds\int_0^\infty ds'\,e^{-ps-qs'}\delta(s-s')\\
&=\frac{2A_k}{p+q}.
\end{aligned}
$$

For clarity about contour signs, introduce the inverse-transform measures

$$
\int_{\mathcal B}\frac{dp}{2\pi i},\qquad
\int_{\mathcal B^*}\frac{dq}{-2\pi i}.
$$

The first [Bromwich inversion formula](../../../../bromwich-inversion-formula.md) contour runs upward on $\operatorname{Re}p=\sigma$; its conjugate contour runs downward on $\operatorname{Re}q=\sigma$. Both measures therefore have the same positive orientation in their real [frequency](../../../../frequency.md) parameters. Combining the averaged equation with $\widehat{\delta f}_k$ yields

$$
\partial_tf_0=\partial_v\left[D(v,t)\partial_vf_0\right],\qquad
D=-\frac e{m_e f_0'}\sum_k(-ik)\langle\delta f_k(t,v)\varphi_k(t)^*\rangle.
$$

At a zero of $f_0'$, the last expression means its continuous coefficient obtained before cancelling $f_0'$. Substitution of the two inverse [Laplace transforms](../../../../laplace-transform.md) and the transformed covariance gives

$$
\boxed{D(v,t)=\frac{e^2}{m_e^2}\sum_k\frac{k^2A_k}{2\pi^2}\int_{\mathcal B}dp\int_{\mathcal B^*}dp'^*\,\frac{e^{(p+p'^*)t}}{(p+ikv)(p+p'^*)\epsilon(p,k)\epsilon(p',k)^*}.}
$$

This is the paper's expression, with the orientation of $dp'^*$ made explicit. Reality follows by pairing $k$ and $-k$. The double integral retains switch-on transients; replacing it by a time-independent [diffusion coefficient](../../../../diffusion-coefficient.md) requires the additional long-time limit in [b](../b.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
