<h1 id="35a/solution">Solution</h1>

↑ **Parent:** [35A](../35a.md)

Label the two atoms in primitive cell $j$ by $u_{2j}$ and $u_{2j+1}$, with $j$ understood modulo $N$ because of the [periodic boundary condition](../../../../../periodic-boundary-conditions.md). Choose the spring between them to have constant $\lambda$. [Newton's second law](../../../../../newton-s-second-law.md) gives

$$
\begin{aligned}
m\ddot u_{2j}
&=\lambda(u_{2j+1}-u_{2j})
+\alpha\lambda(u_{2j-1}-u_{2j}),\\
m\ddot u_{2j+1}
&=\lambda(u_{2j}-u_{2j+1})
+\alpha\lambda(u_{2j+2}-u_{2j+1}).
\end{aligned}
$$

For a longitudinal [normal mode](../../../../../normal-mode.md), put

$$
u_{2j}=A e^{i(2jka-\omega t)},
\qquad
u_{2j+1}=B e^{i((2j+1)ka-\omega t)}.
$$

Periodicity requires $e^{2iNka}=1$, so $k=\pi r/(Na)$. Since the primitive-cell length is $2a$, wavevectors differing by $\pi/a$ describe the same mode, and the first [Brillouin zone](../../../../../brillouin-zone.md) may be chosen as

$$
\boxed{-\frac{\pi}{2a}\leq k<\frac{\pi}{2a}.}
$$

The amplitudes obey

$$
\begin{pmatrix}
\lambda(1+\alpha)-m\omega^2&
-\lambda(e^{ika}+\alpha e^{-ika})\\
-\lambda(e^{-ika}+\alpha e^{ika})&
\lambda(1+\alpha)-m\omega^2
\end{pmatrix}
\begin{pmatrix}A\\B\end{pmatrix}=0.
$$

Setting its [determinant](../../../../../determinant.md) to zero gives the [alternating-spring chain dispersion relation](../../../../../alternating-spring-chain-dispersion-relation.md)

$$
\boxed{
\omega_\pm^2(k)=\frac{\lambda}{m}
\left[1+\alpha\pm
\sqrt{(1-\alpha)^2+4\alpha\cos^2(ka)}\right].}
$$

The lower sign is the [acoustic phonon branch](../../../../../acoustic-phonon-branch.md) and the upper sign is the [optical phonon branch](../../../../../optical-phonon-branch.md).

At the edge of the [Brillouin zone](../../../../../brillouin-zone.md),

$$
\omega_\pm^2=\frac{\lambda}{m}
\left(1+\alpha\pm|1-\alpha|\right),
$$

so the frequency [band gap](../../../../../band-gap.md) is

$$
\boxed{\Delta\omega=
\sqrt{\frac{2\lambda}{m}}\,|1-\sqrt\alpha|.}
$$

It vanishes at $\alpha=1$, when the apparent two-atom primitive cell can be reduced to one atom.

Near the centre of the [Brillouin zone](../../../../../brillouin-zone.md), a [Taylor expansion](../../../../../taylor-expansion.md) gives

$$
\boxed{
\omega_-(k)=
a\sqrt{\frac{2\alpha\lambda}{m(1+\alpha)}}\,|k|
+O(|k|^3),}
$$

and

$$
\boxed{
\omega_+(k)=
\sqrt{\frac{2\lambda(1+\alpha)}m}
\left[1-\frac{\alpha a^2k^2}{2(1+\alpha)^2}
+O(k^4)\right].}
$$

The [group velocity](../../../../../group-velocity.md) of the acoustic branch at long wavelength is the [speed of sound](../../../../../speed-of-sound.md),

$$
\boxed{c_s=a\sqrt{\frac{2\alpha\lambda}{m(1+\alpha)}}.}
$$

<a id="35a/image-dispersion-relation-of-the-alternating-spring-chain"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2-alternating-spring-dispersion.png)

**[Figure 1](#35a/image-dispersion-relation-of-the-alternating-spring-chain). Dispersion relation of the alternating-spring chain**. The acoustic and optical branches for alpha equal to 0.35. The vertical separation at the Brillouin-zone edge is the frequency gap.

## ↑ Ancestors (10)

1. [35A](../35a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
