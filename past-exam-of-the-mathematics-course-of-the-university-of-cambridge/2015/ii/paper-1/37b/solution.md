<h1 id="37b/solution">Solution</h1>

↑ **Parent:** [37B](../37b.md)

Linearized momentum balance is $\rho_0\partial_t\tilde u=-\nabla\tilde p$. For a progressive [acoustic plane wave](../../../../../acoustic-plane-wave.md) $\tilde p=P(\hat k\cdot x-c_0t)$, integration gives

$$
\boxed{\tilde u=\frac{\hat k}{\rho_0c_0}\tilde p}.
$$

The integration constant is zero for the pure wave with no added uniform flow. The instantaneous [acoustic intensity](../../../../../acoustic-energy-flux.md) is $I=\tilde p\tilde u$, the pressure-work energy flux; time-averaged intensity is $\langle I\rangle$. For complex harmonic pressure amplitude $P$, $\langle I\rangle=|P|^2\hat k/(2\rho_0c_0)$.

Use phase convention $e^{i(k_y y-\omega t)}$, with $\omega=kc_0$, $k_y=k\sin\theta$, $k_x=k\cos\theta>0$. Let incident, reflected and transmitted pressure amplitudes be $1,R,T_p$. The two normal velocities at the membrane are $(1-R)\cos\theta/(\rho_0c_0)$ and $T_p\cos\theta/(\rho_0c_0)$, and both equal $-i\omega X_0$. Hence $T_p=1-R$ and $X_0=iT_p\cos\theta/(\rho_0c_0\omega)$. Only normal velocity is matched for an inviscid fluid; tangential velocities need not agree.

Put $D_m=k^2(mc_0^2-T\sin^2\theta)$. The dynamic condition is $-D_mX_0+T_p-(1+R)=0$, or $-D_mX_0-2R=0$. Since $D_m\cos\theta/(\rho_0c_0\omega)=1/\alpha$, elimination gives

$$
\boxed{R=\frac1{1+2i\alpha},\qquad T_p=\frac{2i\alpha}{1+2i\alpha}}.
$$

Complex conjugation gives the amplitudes for the opposite time-phase convention. At zero $D_m$, the formulas have the limiting values $R=0,T_p=1$ even though $\alpha$ itself is then infinite. A strongly inertial membrane has $\alpha\to0$, giving almost total reflection.

For real $\alpha$, $|R|^2+|T_p|^2=1$. Thus the incoming net normal energy flux is $\cos\theta(1-|R|^2)/(2\rho_0c_0)$, equal to the transmitted flux $\cos\theta|T_p|^2/(2\rho_0c_0)$. **Time-averaged energy flux is conserved**: the lossless membrane stores and returns energy but has no mean dissipation.

## ↑ Ancestors (10)

1. [37B](../37b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
