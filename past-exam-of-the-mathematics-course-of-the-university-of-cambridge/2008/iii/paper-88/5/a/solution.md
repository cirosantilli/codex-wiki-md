<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $k=|\mathbf k_i|$ for the background wavenumber and $\psi_i=e^{i\mathbf k_i\cdot\mathbf r}$. The [Helmholtz equation](../../../../../../helmholtz-equation.md) gives

$$
(\Delta+k^2)\psi_s=-k^2(n^2-1)\psi.
$$

The [Born approximation for scalar wave scattering](../../../../../../born-approximation-for-scalar-wave-scattering.md) replaces $\psi$ in this source term by $\psi_i$. For the question's contrast $V=-k(n-1)$, also linearize $n^2-1\simeq2(n-1)$. Since $(\Delta+k^2)e^{ikR}/R=-4\pi\delta$, the outgoing scattered field is

$$
\boxed{\psi_s(\mathbf r)=-\frac{k}{2\pi}\int_D V(\mathbf r')
\frac{e^{ik|\mathbf r-\mathbf r'|}}{|\mathbf r-\mathbf r'|}
e^{i\mathbf k_i\cdot\mathbf r'}\,d^3r'.}
$$

Without the small-contrast linearization, replace $V$ by $-k(n^2-1)/2$ in this formula.

Apply the [Weyl plane-wave representation](../../../../../../weyl-plane-wave-representation.md). For an observation plane wholly above or below $D$, put $\sigma=+1$ or $-1$, respectively, and choose $m=\sqrt{1-p^2-q^2}$ with nonnegative imaginary part. Define $\widetilde V(\boldsymbol\kappa)=\int_DV(\mathbf r')e^{-i\boldsymbol\kappa\cdot\mathbf r'}d^3r'$. Substitution gives

$$
\boxed{\psi_s(\mathbf r)=-\frac{ik^2}{4\pi^2}\int\frac{dp\,dq}{m}
 e^{ik(px+qy+\sigma mz)}
\widetilde V(kp-k_{i,x},kq-k_{i,y},\sigma km-k_{i,z}).}
$$

For the lower observation plane the vertical phase has the opposite sign. This follows from the absolute separation $|z-z'|$ in the Weyl identity; its version with $z-z'$ alone applies only above the sources.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 88](../../../paper-88-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
