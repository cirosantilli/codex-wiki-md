<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Uniform $\rho_0,p_0,$ and $\mathbf B_0=B_0\widehat{\mathbf z}$ obey the unperturbed [ideal magnetohydrodynamics](../../../../../../ideal-magnetohydrodynamics.md) equations when

$$
\boxed{\mathbf v_0=-q\Omega_0x\widehat{\mathbf y}}.
$$

Indeed $(\mathbf v_0\mathbin\cdot\nabla)\mathbf v_0=0$, while the Coriolis and tidal terms cancel:

$$
-2\Omega_0\widehat{\mathbf z}\times\mathbf v_0
+2q\Omega_0^2x\widehat{\mathbf x}=0.
$$

For perturbations proportional to $e^{i(\omega t-kz)}$, the horizontal velocity and magnetic perturbations decouple from the compressive variables. Their linear equations are

$$
i\omega v_x-2\Omega_0v_y
=-ik\frac{B_0}{4\pi\rho_0}B_x,
$$



$$
i\omega v_y+(2-q)\Omega_0v_x
=-ik\frac{B_0}{4\pi\rho_0}B_y,
$$



$$
i\omega B_x=-ikB_0v_x,
\qquad
i\omega B_y=-q\Omega_0B_x-ikB_0v_y.
$$

Eliminating $B_x,B_y,v_x,v_y$ and writing the [Alfvén speed](../../../../../../alfven-speed.md) as $v_A^2=B_0^2/(4\pi\rho_0)$ gives

$$
\boxed{
\omega^4-omega^2\left[2k^2v_A^2+2(2-q)\Omega_0^2\right]
+k^2v_A^2\left(k^2v_A^2-2q\Omega_0^2\right)=0}.
$$

Since $d\Omega_0^2/d\log r=-2q\Omega_0^2$, a root has $\omega^2<0$ precisely when the constant term is negative:

$$
\boxed{k^2v_A^2+\frac{d\Omega_0^2}{d\log r}<0}.
$$

This is the [magnetorotational instability](../../../../../../magnetorotational-instability.md) criterion.

For a [circular Kepler orbit](../../../../../../circular-kepler-orbit.md), $q=3/2$. With $K=k^2v_A^2$, the unstable branch is

$$
\omega_-^2=K+\frac12\Omega_0^2
-\Omega_0\sqrt{4K+\frac14\Omega_0^2}.
$$

Minimizing it gives

$$
K_{\max}=\frac{15}{16}\Omega_0^2,
\qquad
\omega_-^2=-\frac9{16}\Omega_0^2,
$$

and hence

$$
\boxed{|\omega_{\max}|=\frac34\Omega_0}.
$$

The e-folding time is of order the dynamical time, so the growth is rapid: several e-foldings occur in one orbit.

Instability requires $k^2v_A^2<3\Omega_0^2$, making the [critical wavelength of the magnetorotational instability](../../../../../../critical-wavelength-of-the-magnetorotational-instability.md)

$$
\lambda_{\rm crit}=\frac{2\pi v_A}{\sqrt3\Omega_0}.
$$

For a thin isothermal disk, $H=c_{s,0}/\Omega_0$. Setting $\lambda_{\rm crit}=2H$ gives $v_A^2=3c_{s,0}^2/\pi^2$, and therefore

$$
\boxed{B_{0,\rm crit}^2=4\pi\rho_0v_A^2
=\frac{12}{\pi}\rho_0c_{s,0}^2}.
$$

Above this field strength the shortest unstable vertical MRI wavelength exceeds the full disk thickness, so no such vertical mode fits inside the disk. Magnetic tension then stabilizes this local mode; the result corresponds to a magnetic-to-gas pressure ratio $B^2/(8\pi p)=3/(2\pi^2)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
