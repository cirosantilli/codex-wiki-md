<h1 id="38a/solution">Solution</h1>

↑ **Parent:** [38A](../38a.md)

Linearized continuity and Euler equations about a uniform resting inviscid fluid are $\rho'_t+\rho_0\nabla\cdot\mathbf u=0$ and $\rho_0\mathbf u_t=-\nabla p'$. For a velocity potential $\mathbf u=\nabla\phi$ and sound-speed relation $p'=c^2\rho'$, integration of Euler's equation fixes the temporal gauge so $p'=-\rho_0\phi_t$. Substitution into continuity gives

$$
\boxed{\phi_{tt}=c^2\nabla^2\phi,\qquad p'=-\rho_0\phi_t.}
$$

Use complex amplitudes with time factor $e^{i\omega t}$. The outgoing wave in fluid two is $\Phi_2(x)=Ae^{-ik_2x}$, with $k_i=\omega/c_i$. Write $\Phi_1=C\cos(k_1x)+D\sin(k_1x)$. Continuity of pressure and normal velocity at zero gives

$$
C=(\rho_2/\rho_1)A,\qquad D=-i(c_1/c_2)A.
$$

The piston velocity is $i\omega\epsilon$, so $\Phi_1'(-L)=i\omega\epsilon$. With $\theta=\omega L/c_1$, this gives

$$
A\bigl[(\rho_2/\rho_1)\sin\theta-i(c_1/c_2)\cos\theta\bigr]
=i\epsilon c_1,
$$

and hence the requested amplitude is

$$
\boxed{A=-\epsilon c_1\left[(c_1/c_2)\cos\theta
+i(\rho_2/\rho_1)\sin\theta\right]^{-1}.}
$$

For complex pressure and velocity amplitudes, the mean [acoustic energy flux](../../../../../acoustic-energy-flux.md) is $\tfrac12\operatorname{Re}(PU^*)$. Here $P=-i\omega\rho_2\Phi_2$ and $U=-ik_2\Phi_2$, so

$$
\boxed{\langle\mathcal F\rangle=
\frac{\rho_2\omega^2\epsilon^2c_1^2}{2c_2}
\left[(c_1/c_2)^2\cos^2\theta+(\rho_2/\rho_1)^2\sin^2\theta\right]^{-1}.}
$$

For $\rho_2\ll\rho_1$ and comparable sound speeds, weak transmission loads the finite segment. There are narrow large-flux resonances near $\theta=(n+1/2)\pi$, separated by $\Delta L=\pi c_1/\omega$. The off-resonance scale is proportional to $\rho_2$, while peak flux is proportional to $\rho_1^2/\rho_2$; the angular width is of order $(\rho_2/\rho_1)(c_2/c_1)$. These amplified solutions remain within linear acoustics only when the resulting wave amplitudes are small.

## ↑ Ancestors (10)

1. [38A](../38a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
