<h1 id="17a/solution">Solution</h1>

↑ **Parent:** [17A](../17a.md)

For inviscid flow with a conservative body-force potential $\Phi$, the [Euler momentum equation](../../../../../euler-equations-for-an-inviscid-fluid.md) and the identity $(\mathbf u\cdot\nabla)\mathbf u=\nabla(|\mathbf u|^2/2)-\mathbf u\times(\nabla\times\mathbf u)$ apply. In an irrotational region write $\mathbf u=\nabla\phi$. For constant density they give

$$
\nabla\left(\phi_t+\tfrac12|\nabla\phi|^2+p/\rho+\Phi\right)=0,
\qquad
\boxed{\phi_t+\tfrac12|\mathbf u|^2+p/\rho+\Phi=C(t).}
$$

This is the [Unsteady Bernoulli equation](../../../../../unsteady-bernoulli-equation.md); its constant is spatially uniform, with time-dependent gauge absorbed into $\phi$ if desired.

For the intended [linearly elastic balloon discharge](../../../../../linearly-elastic-balloon-discharge.md) model, take an initially stationary, inviscid plug of water in the constant-area tube. Put $B=\pi a^2$ and $p_{\rm in}-p_{\rm atm}=KV$ with $K>0$. At the two tube ends the speeds are equal, so their kinetic terms cancel in the Bernoulli difference. Since $\phi(L)-\phi(0)=Lu$, this gives

$$
\rho L\dot u=KV,\qquad \dot V=-Bu.
$$

Hence $\ddot V+\Omega^2V=0$, where $\Omega^2=KB/(\rho L)$. With $V(0)=V_0$ and $u(0)=0$,

$$
V=V_0\cos\Omega t,\qquad u=\frac{\Omega V_0}{B}\sin\Omega t.
$$

Thus

$$
\boxed{T_{\rm empty}=\frac\pi{2\Omega}=\frac\pi2\sqrt{\frac{\rho L}{K\pi a^2}},\qquad
u_{\max}=\frac{\Omega V_0}{\pi a^2}=V_0\sqrt{\frac{K}{\rho L\pi a^2}}.}
$$

Acceleration stays positive until emptying, so the maximum speed is reached at that instant. The time is independent of initial volume, while the maximum speed is not.

The initial-rest condition is implicit in the claimed volume independence, rather than specified in the text. For an independently prescribed positive initial speed $u_0$, the first zero instead occurs at $\Omega^{-1}\arctan[\Omega V_0/(Bu_0)]$. The calculation also takes the given balloon pressure as the pressure directly at the tube entrance; a reservoir-to-exit kinetic-head or entrance-loss model would add other terms and is not this equal-speed tube model.

## ↑ Ancestors (10)

1. [17A](../17a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
