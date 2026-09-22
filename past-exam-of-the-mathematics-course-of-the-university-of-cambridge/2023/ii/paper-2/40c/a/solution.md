<h1 id="40c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $k_S=\omega/c_S$ and $k_P=\omega/c_P$. [Snell law for elastic waves](../../../../../../snell-law-for-elastic-waves.md) fixes the reflected waves' common tangential wavenumber:

$$
k_S\sin\theta=k_P\sin\phi,
\qquad
\sin\phi=\frac{c_P}{c_S}\sin\theta.
$$

Choose the reflected [SV-wave](../../../../../../sv-wave.md) and converted reflected [P wave](../../../../../../p-wave.md) as

$$
\mathbf u_{RS}
=\operatorname{Re}\left\{
R(\cos\theta,0,\sin\theta)
 e^{ik_S(x\sin\theta-z\cos\theta)-i\omega t}
\right\},
$$



$$
\mathbf u_{RP}
=\operatorname{Re}\left\{
T(\sin\phi,0,-\cos\phi)
 e^{ik_P(x\sin\phi-z\cos\phi)-i\omega t}
\right\}.
$$

The polarizations are respectively perpendicular and parallel to their [wavevectors](../../../../../../wavevector.md). Phase matching makes all three exponential factors equal at $z=0$. The [rigid boundary condition for an elastic wave](../../../../../../rigid-boundary-condition-for-an-elastic-wave.md) $\mathbf u_I+\mathbf u_{RS}+\mathbf u_{RP}=0$ there gives

$$
\cos\theta(1+R)+T\sin\phi=0,
$$



$$
-\sin\theta+R\sin\theta-T\cos\phi=0.
$$

Solving this two-by-two [linear system](../../../../../../system-of-linear-equations.md) yields

$$
\boxed{R=-\frac{\cos(\theta+\phi)}{\cos(\theta-\phi)}},
\qquad
\boxed{T=-\frac{\sin2\theta}{\cos(\theta-\phi)}}.
$$

These fields give the [Reflection of an SV-wave from a rigid plane](../../../../../../reflection-of-an-sv-wave-from-a-rigid-plane.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [40C](../../40c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
