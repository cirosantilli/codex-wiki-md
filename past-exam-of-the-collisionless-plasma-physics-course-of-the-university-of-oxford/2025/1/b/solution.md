<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Faraday law](../../../../faraday-s-law-of-induction.md) and [Ampere-Maxwell law](../../../../ampere-s-circuital-law.md) give $\delta\mathbf B=(c/\omega)\mathbf k\times\delta\mathbf E$ and

$$
\mathbf k\times(\mathbf k\times\delta\mathbf E)+\frac{\omega^2}{c^2}\boldsymbol\epsilon\cdot\delta\mathbf E=0.
$$

With [refractive index](../../../../refractive-index.md) $n=kc/\omega$, the [linear system](../../../../system-of-linear-equations.md) is therefore

$$
\begin{pmatrix}
S-n^2\cos^2\theta&ig&n^2\sin\theta\cos\theta\\
-ig&S-n^2&0\\
n^2\sin\theta\cos\theta&0&P-n^2\sin^2\theta
\end{pmatrix}\delta\mathbf E=0.
$$

Set

$$
\boxed{R=S-g,\qquad L=S+g,\qquad RL=S^2-g^2.}
$$

Here $R$ labels the [cold-plasma right-handed wave](../../../../cold-plasma-right-handed-wave.md) and $L$ the [cold-plasma left-handed wave](../../../../cold-plasma-left-handed-wave.md), with their [polarizations](../../../../polarization-waves.md) fixed explicitly in [d](../d.md). In the [electron](../../../../electron.md)-only response,

$$
R=1-\frac{\omega_{pe}^2}{\omega(\omega-\Omega_e)},\qquad
L=1-\frac{\omega_{pe}^2}{\omega(\omega+\Omega_e)}.
$$

Writing $N=n^2$, expansion of the [determinant](../../../../determinant.md) yields the [dispersion relation](../../../../dispersion-relation-split.md)

$$
A N^2-BN+C=0,\quad
A=S\sin^2\theta+P\cos^2\theta,\quad
B=RL\sin^2\theta+PS(1+\cos^2\theta),\quad C=PRL.
$$

Equivalently,

$$
P(N-R)(N-L)\cos^2\theta+(SN-RL)(N-P)\sin^2\theta=0.
$$

Division gives

$$
\boxed{\tan^2\theta=-\frac{P(n^2-R)(n^2-L)}{(Sn^2-RL)(n^2-P)}.}
$$

The undivided [determinant](../../../../determinant.md) equation remains valid when this rational form has simultaneous zero factors.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the collisionless plasma physics course of the University of Oxford](../../../split.md)
5. [Collisionless plasma physics course of the University of Oxford](../../../../collisionless-plasma-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
