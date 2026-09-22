<h1 id="36b/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take the plane of incidence to be the $xy$-plane, so all three electric polarizations point along $z$. Write their signed scalar amplitudes as $E_I,E_R,E_T$. Tangential-$E$ continuity gives

$$
E_I+E_R=E_T.
$$

For each plane wave,

$$
H=\frac1{\mu\omega}k\times E.
$$

Continuity of its tangential component gives

$$
n_-\cos\theta_I(E_I-E_R)
=n_+\cos\theta_T E_T,
$$

where the common proportionality between $|k|$ and $n$ cancels. Solving the two equations gives the [transverse-electric Fresnel reflection coefficient](../../../../../../transverse-electric-fresnel-reflection-coefficient.md)

$$
\frac{E_R}{E_I}
=\frac{n_-\cos\theta_I-n_+\cos\theta_T}
{n_-\cos\theta_I+n_+\cos\theta_T}.
$$

Using Snell's law to eliminate $\theta_T$,

$$
n_+\cos\theta_T
=\sqrt{n_+^2-n_-^2\sin^2\theta_I}.
$$

Since $\epsilon_+>\epsilon_-$ and $\mu$ is common, $n_+>n_-$. Therefore

$$
(n_+\cos\theta_T)^2-(n_-\cos\theta_I)^2
=n_+^2-n_-^2>0.
$$

The numerator is consequently strictly negative throughout  
$0\leq\theta_I\leq\pi/2$, and

$$
\boxed{
\frac{|E_R|}{|E_I|}
=
\frac{
\sqrt{n_+^2-n_-^2\sin^2\theta_I}
-n_-\cos\theta_I}
{
\sqrt{n_+^2-n_-^2\sin^2\theta_I}
+n_-\cos\theta_I}
>0}.
$$

**Thus transverse-electric polarization has no Brewster angle in this setting.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [36B](../../36b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
