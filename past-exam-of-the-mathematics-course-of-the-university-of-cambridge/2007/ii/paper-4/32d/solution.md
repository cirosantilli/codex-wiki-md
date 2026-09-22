<h1 id="32d/solution">Solution</h1>

↑ **Parent:** [32D](../32d.md)

The [Pauli matrices](../../../../../pauli-matrices.md) obey $(\mathbf n\cdot\boldsymbol\sigma)^2=I$. Expanding the exponential into even and odd powers gives the [time-evolution operator](../../../../../time-evolution-operator.md)

$$
\boxed{U(t)=e^{-iHt/\hbar}
=I\cos(\gamma Bt/2)+i\mathbf n\cdot\boldsymbol\sigma\sin(\gamma Bt/2).}
$$

For orthogonal states the identity contribution vanishes, so the transition probability is $|\langle\chi'|\mathbf n\cdot\boldsymbol\sigma|\chi\rangle|^2\sin^2(\gamma Bt/2)$. For spin up to spin down in a static field $(B_x,0,B_z)$, only $\sigma_x$ has the required matrix element. Hence

$$
\boxed{P_{\uparrow\to\downarrow}(t)=\frac{B_x^2}{B_x^2+B_z^2}
\sin^2\left(\frac{\gamma\sqrt{B_x^2+B_z^2}\,t}{2}\right).}
$$

For the weak rotating transverse field, take $H_0=-\hbar\gamma B_z\sigma_z/2$. The unperturbed energies give $E_\downarrow-E_\uparrow=\hbar\gamma B_z$. The perturbation matrix element is $\langle\downarrow|V(t)|\uparrow\rangle=-\hbar\gamma A e^{i\alpha t}/2$. Thus first-order perturbation theory gives

$$
a_\downarrow(t)=\frac{i\gamma A}{2}\int_0^t e^{i(\gamma B_z+\alpha)s}\,ds
=\frac{\gamma A}{2\Omega}(e^{i\Omega t}-1),\qquad \Omega=\gamma B_z+\alpha.
$$

Squaring its magnitude yields

$$
\boxed{P_{\uparrow\to\downarrow}\approx
\left(\frac{\gamma A}{\gamma B_z+\alpha}\right)^2
\sin^2\left(\frac{(\gamma B_z+\alpha)t}{2}\right).}
$$

The hypothesis is $|\gamma A|\ll|\Omega|$, excluding resonance. At $\alpha=0$ this is the leading weak-$A$ expansion of the exact static-field formula with $B_x=A$. For extremely long times, a small higher-order frequency correction can accumulate phase, so first-order perturbation is not a uniform approximation on arbitrarily long time scales.

## ↑ Ancestors (10)

1. [32D](../32d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
