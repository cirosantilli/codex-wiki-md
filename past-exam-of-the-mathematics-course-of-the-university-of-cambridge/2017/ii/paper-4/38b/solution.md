<h1 id="38b/solution">Solution</h1>

↑ **Parent:** [38B](../38b.md)

Substitution of $e^{i(kx-\omega t)}$ gives

$$
\boxed{\omega(k)=-\frac{\beta k}{k^2+\ell^2},\qquad c(k)=\frac\omega k=-\frac\beta{k^2+\ell^2},\qquad
c_g(k)=\omega'(k)=\frac{\beta(k^2-\ell^2)}{(k^2+\ell^2)^2}.}
$$

The [phase velocity](../../../../../phase-velocity.md) is negative for all nonzero [wavenumbers](../../../../../wavenumber.md), so crests travel left. The [group velocity](../../../../../group-velocity.md) is negative for $|k|<\ell$, zero at $|k|=\ell$, and positive for $|k|>\ell$. Its minimum is $-\beta/\ell^2$ at zero and maximum $\beta/(8\ell^2)$ at $|k|=\sqrt3\ell$; it tends to zero from above at infinity. The odd [dispersion relation](../../../../../dispersion-relation.md) has extrema at $k=\pm\ell$, with $\omega(\ell)=-\beta/(2\ell)$.

<a id="38b/image-rossby-dispersion-phase-velocity-and-group-velocity-in-dimensionless-variables"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4-rossby.png)

**[Figure 6](#38b/image-rossby-dispersion-phase-velocity-and-group-velocity-in-dimensionless-variables). Rossby dispersion, phase velocity and group velocity in dimensionless variables**.

The Fourier solution is $\varphi(x,t)=\int_{\mathbb R}A(k)e^{i[kx-\omega(k)t]}\,dk$. The stationary-phase statements require enough amplitude regularity and decay, for example $A$ smooth and rapidly decreasing; realness and evenness alone do not guarantee a convergent integral or a stationary-phase expansion. For $x=Vt$, set $\Phi_V(k)=kV-\omega(k)$ and solve $\omega'(k)=V$ implicitly. 

## ↑ Ancestors (10)

1. [38B](../38b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
