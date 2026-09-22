<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take $\omega>0$, with time convention $e^{-i\omega t}$, and use the [Fourier transform](../../../../../fourier-transform.md) pair $\widehat h(k)=\int h(x)e^{-ikx}\,dx$, $h(x)=(2\pi)^{-1}\int\widehat h(k)e^{ikx}\,dk$. For an [acoustic velocity potential](../../../../../acoustic-velocity-potential.md), $\mathbf u=\nabla\phi$ and $p=-\rho_0\phi_t$. Its harmonic amplitude solves the [Helmholtz equation](../../../../../helmholtz-equation.md). The outgoing Fourier component has the form

$$
\widehat\phi(k,y)=A(k)e^{-\gamma y},\qquad \gamma^2=k^2-k_0^2,\qquad k_0=\omega/c_0.
$$

The [outgoing acoustic square-root branch](../../../../../outgoing-acoustic-square-root-branch.md) is fixed by decay for evanescent components and upward radiation for propagating components:

$$
\gamma(k)=\begin{cases}\sqrt{k^2-k_0^2}>0,&|k|>k_0,\\-i\sqrt{k_0^2-k^2},&|k|<k_0.\end{cases}
$$

A precise causal prescription is to replace $\omega$ by $\omega+i\sigma$, $\sigma>0$, select $\operatorname{Re}\gamma>0$ for real $k$, invert on the real $k$ axis, and take $\sigma\downarrow0$. It corresponds to switching on the forcing from the remote past. The limiting inversion contour $C$ passes below the positive outgoing surface-wave pole and above the negative one. The branch points are approached with the same causal prescription; analytic continuation during contour deformation must remain on this sheet. A principal real square root with positive imaginary part inside the acoustic interval would produce incoming sound and the wrong solution.

The [elastic membrane](../../../../../elastic-membrane.md)'s normal [velocity](../../../../../velocity.md) equals the fluid velocity at the boundary, so $-\gamma A=-i\omega\widehat\eta$. Consequently

$$
A=\frac{i\omega}{\gamma}\widehat\eta,\qquad \widehat p(k,0)=-\frac{\rho_0\omega^2}{\gamma}\widehat\eta.
$$

The [elastic membrane](../../../../../elastic-membrane.md) balance therefore gives

$$
\left(Tk^2-m\omega^2-\frac{\rho_0\omega^2}{\gamma}\right)\widehat\eta=F.
$$

Writing $D=(Tk^2-m\omega^2)\gamma-\rho_0\omega^2$, the [one-sided fluid-loaded membrane radiation](../../../../../one-sided-fluid-loaded-membrane-radiation.md) formulas are

$$
\boxed{\eta(x,t)=\frac F{2\pi}\int_C\frac{\gamma e^{ikx-i\omega t}}{D(k,\omega)}\,dk,\qquad \phi(x,y,t)=\frac{i\omega F}{2\pi}\int_C\frac{e^{ikx-\gamma y-i\omega t}}{D(k,\omega)}\,dk.}
$$

The sign of the fluid term describes positive [added mass of an evanescent fluid layer](../../../../../added-mass-of-an-evanescent-fluid-layer.md), not negative inertia.

For $0<\theta<\pi$, the acoustic [saddle point](../../../../../saddle-point.md) is $k_s=k_0\cos\theta$, with $\gamma_s=-ik_0\sin\theta$. Applying the stated [method of steepest descent](../../../../../method-of-steepest-descent.md) result gives

$$
\phi_{\rm rad}\sim i\omega F\sqrt{\frac{k_0}{2\pi r}}\frac{\sin\theta}{D_s}e^{ik_0r-i\omega t-i\pi/4},\qquad D_s=-\rho_0\omega^2-ik_0\sin\theta(Tk_0^2\cos^2\theta-m\omega^2).
$$

Since $p=i\rho_0\omega\phi$ in amplitude notation, the angular [acoustic directivity](../../../../../acoustic-directivity.md) of the pressure, apart from angle-independent factors, is

$$
\boxed{\mathcal D(\theta)=\frac{\sin\theta}{\sqrt{\rho_0^2+k_0^2\sin^2\theta\,[m-(T/c_0^2)\cos^2\theta]^2}}.}
$$

The intensity directivity is proportional to $\mathcal D^2$. This cylindrical radiating field has amplitude of order $r^{-1/2}$. The formula is for fixed interior angles; grazing-angle limits require a separate uniform approximation.

For real $k>k_0$, $\gamma$ is positive, $D\to-\rho_0\omega^2$ as $k\downarrow k_0$, and $D\to+\infty$ as $k\to\infty$. A root exists. A root also requires $Tk^2-m\omega^2>0$. In that range,

$$
D_k=2Tk\gamma+(Tk^2-m\omega^2)\frac{k}{\gamma}>0,
$$

so the root is unique. Evenness supplies the second root, $-k_*$. There are no real roots inside $|k|<k_0$: the fluid-loading term is real and nonzero while the other term is purely imaginary. Thus **there are exactly two real physical-sheet roots, $\pm k_*$, for nonzero forcing frequency, positive [elastic-sheet tension](../../../../../elastic-sheet-tension.md) and positive fluid [mass density](../../../../../density.md)**. The zero-frequency static limit is not a two-distinct-root statement.

These roots are counterpropagating [evanescent acoustic surface waves](../../../../../evanescent-acoustic-surface-wave.md) coupled to the membrane:

$$
\omega^2\left(m+\frac{\rho_0}{\gamma_*}\right)=Tk_*^2,\qquad \gamma_*=\sqrt{k_*^2-k_0^2}>0.
$$

Their normal profiles decay as $e^{-\gamma_*y}$, and their phase speed is below both $c_0$ and the vacuum membrane speed. They matter for the [elastic membrane](../../../../../elastic-membrane.md) motion and for observations near its surface, but are not automatically part of the leading far-field radiation. A residue is picked up only when the causal contour deformation crosses its pole; at fixed $y/r>0$ its magnitude is exponentially small, $e^{-\gamma_*r\sin\theta}$.

For example, in the right half-plane put $k=k_0\cos\zeta$, $\gamma=-ik_0\sin\zeta$ and $k_*=k_0\cosh a$. The pole is at $\zeta=ia$ and the saddle at $\zeta=\theta$. The steepest-descent path has $\operatorname{Re}\cos(\zeta-\theta)=1$. At the pole height its left branch has real coordinate $\theta-\arccos(\operatorname{sech}a)$; comparing it with the original contour just to the right of the pole shows that its residue is crossed for

$$
0<\theta<\theta_s,\qquad \theta_s=\arccos(k_0/k_*).
$$

The analogous sector lies near $\theta=\pi$ for the negative pole. This is why the existence of real dispersion zeros alone does not make their residues relevant in every observation direction.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
