<h1 id="39a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $Z_j=\rho_jc_j$, $k_j=\omega/c_j$, and $\phi=k_1L$. Use the harmonic convention $e^{-i\omega t}$ and write the pressure and velocity amplitudes as

$$
\begin{array}{lll}
x<0:&p=e^{ik_0x}+Re^{-ik_0x},&u=Z_0^{-1}(e^{ik_0x}-Re^{-ik_0x}),\\
0<x<L:&p=Ae^{ik_1x}+Be^{-ik_1x},&u=Z_1^{-1}(Ae^{ik_1x}-Be^{-ik_1x}),\\
x>L:&p=Te^{ik_0(x-L)},&u=Z_0^{-1}Te^{ik_0(x-L)}.
\end{array}
$$

Continuity of pressure and normal velocity at both interfaces is equivalently the layer transfer relation

$$
\binom{p(0)}{u(0)}=
\begin{pmatrix}
\cos\phi&-iZ_1\sin\phi\\
-iZ_1^{-1}\sin\phi&\cos\phi
\end{pmatrix}
\binom{p(L)}{u(L)}.
$$

Substituting $p(0)=1+R$, $u(0)=(1-R)/Z_0$, $p(L)=T$, and $u(L)=T/Z_0$, then adding the two resulting equations, gives

$$
2=T\left[2\cos\phi-i\left(\lambda+\lambda^{-1}\right)\sin\phi\right],
\qquad
\lambda=\frac{Z_1}{Z_0}.
$$

Hence the [acoustic transmission through a uniform layer](../../../../../../acoustic-transmission-through-a-uniform-layer.md) is

$$
\boxed{|T|=\left[\cos^2(k_1L)+\frac14(\lambda+\lambda^{-1})^2\sin^2(k_1L)\right]^{-1/2}.}
$$

For either $\lambda\ll1$ or $\lambda\gg1$, the strong [acoustic impedance](../../../../../../acoustic-impedance.md) mismatch makes transmission small except near $k_1L=n\pi$, where $|T|=1$. Away from those resonances,

$$
|T|\sim\frac{2\lambda}{|\sin k_1L|}\quad(\lambda\ll1),
\qquad
|T|\sim\frac{2}{\lambda|\sin k_1L|}\quad(\lambda\gg1).
$$

At the antiresonant points $k_1L=(n+\tfrac12)\pi$, the minimum is $2/(\lambda+\lambda^{-1})$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [39A](../../39a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
