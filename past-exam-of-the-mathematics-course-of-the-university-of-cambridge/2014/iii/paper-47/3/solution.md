<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the [physical rapidity strip](../../../../../physical-rapidity-strip.md) $0<\operatorname{Im}\vartheta<\pi$ for [poles](../../../../../pole.md) of the two-body [S-matrix](../../../../../s-matrix.md), and write $\vartheta$ for scattering [rapidity](../../../../../rapidity.md) to distinguish it from the theta angle in question 2. A denominator in the kink-antikink product vanishes at

$$
\vartheta=iu_k,\qquad u_k=\pi\left(1-\frac{k}{n}\right),\qquad k=1,\ldots,n-1.
$$

No numerator cancels these [poles](../../../../../pole.md). For two equal-mass constituents with [rapidities](../../../../../rapidity.md) $\chi\pm iu_k/2$, their [four-momentum](../../../../../four-momentum.md) vectors sum to

$$
M(\cosh(\chi+iu_k/2),\sinh(\chi+iu_k/2))
+M(\cosh(\chi-iu_k/2),\sinh(\chi-iu_k/2))
=2M\cos(u_k/2)(\cosh\chi,\sinh\chi).
$$

This gives the [relativistic bound-state mass from a rapidity pole](../../../../../relativistic-bound-state-mass-from-a-rapidity-pole.md). The ordered [breather](../../../../../breather.md) spectrum is

$$
\boxed{m_k=2M\sin\frac{k\pi}{2n},\qquad k_{\max}=n-1.}
$$

It increases strictly with $k$. The hypothetical $k=n$ state would lie at the two-kink threshold $2M$ and is not a [bound state](../../../../../bound-state.md); it is absent from the [pole](../../../../../pole.md) product. At these couplings $M=mn/\pi$ and $\beta^2=8\pi/(n+1)$. In particular $m_1\to m$ at weak coupling $n\to\infty$. This is the [Sine-Gordon breather spectrum at reflectionless couplings](../../../../../sine-gordon-breather-spectrum-at-reflectionless-couplings.md). At $n=1$ there are no [breathers](../../../../../breather.md); the subsequent processes involving a physical $\mathcal B_2$ require $n\geq3$.

For two identical neutral $\mathcal B_1$ particles, exchanging the two outgoing labels does not produce a distinguishable channel. In one spatial dimension the elastic final momenta are the incoming pair, up to interchange. Thus there is one scalar identical-particle amplitude, rather than separately observable transmission and reflection amplitudes.

Put $a=\pi/(2n)$, so the basic amplitude uses $\sin(2a)$. Its [poles](../../../../../pole.md) in the physical strip occur at $\vartheta=2ia$ and $\vartheta=i(\pi-2a)$. The first is the direct bound-state [pole](../../../../../pole.md). Choosing constituent [rapidities](../../../../../rapidity.md) $\chi\pm ia$ gives real total energy-momentum

$$
p_1+p_2=2m_1\cos a\,(\cosh\chi,\sinh\chi).
$$

Since $m_1=2M\sin a$,

$$
\boxed{2m_1\cos a=2M\sin(2a)=m_2.}
$$

Both [energy](../../../../../energy.md) and [momentum](../../../../../momentum.md) therefore match an [on shell](../../../../../on-shell.md) $\mathcal B_2$ with [rapidity](../../../../../rapidity.md) $\chi$. The complementary [pole](../../../../../pole.md) is its crossed-channel partner. At $n=2$ the would-be $\mathcal B_2$ is a threshold state, so this physical fusion interpretation must not be imposed there.

The [bound-state fusion of factorized S-matrices](../../../../../bound-state-fusion-of-factorized-s-matrices.md) treats a bound particle as its [on shell](../../../../../on-shell.md) constituents with analytically continued [rapidities](../../../../../rapidity.md). If equal-mass particles $A,A$ fuse to $C$ at relative [rapidity](../../../../../rapidity.md) $iu$, use constituent [rapidities](../../../../../rapidity.md) $\chi\pm iu/2$. To scatter a third particle $D$ off $C$, multiply its [scattering amplitudes](../../../../../scattering-amplitude.md) with each constituent and take the bound-state residue or projection in the constituent channel. For a scalar amplitude this gives

$$
S_{C,D}(\chi-\chi_D)=
S_{A,D}(\chi-\chi_D+iu/2)S_{A,D}(\chi-\chi_D-iu/2).
$$

For particles with internal indices, the product is projected using the bound-state coupling tensors. The heuristic reason is [factorized scattering](../../../../../factorized-scattering.md): conserved higher charges prevent particle production and fix the [rapidity](../../../../../rapidity.md) data, so the third particle scatters through the constituents by successive two-body processes. Consistency of different orders is the [Yang-Baxter equation](../../../../../yang-baxter-equation.md). Without integrability, an independent three-body interaction would invalidate this simple bootstrap product.

For $\mathcal B_2=(\mathcal B_1\mathcal B_1)$, the constituent shifts are $\pm ia$, giving

$$
\boxed{S_{2,1}(\vartheta)=S_{1,1}(\vartheta+ia)S_{1,1}(\vartheta-ia).}
$$

It is useful to write this [Sine-Gordon breather fusion amplitude](../../../../../sine-gordon-breather-fusion-amplitude.md) in explicitly factorized form:

$$
\boxed{S_{2,1}(\vartheta)=
\frac{\sinh\vartheta+i\sin a}{\sinh\vartheta-i\sin a}
\frac{\sinh\vartheta+i\sin(3a)}{\sinh\vartheta-i\sin(3a)}.}
$$

To check the reduction, put $z=\sinh\vartheta$. Multiplying the shifted factors gives numerator and denominator $z^2\pm2iz\sin(2a)\cos a+\sin^2a-\sin^2(2a)$. Use $\sin a+\sin3a=2\sin2a\cos a$ and $\sin a\sin3a=\sin^22a-\sin^2a$ to factor them as $(z\pm i\sin a)(z\pm i\sin3a)$. The product tends to one at large positive real [rapidity](../../../../../rapidity.md), fixing its overall phase in this bootstrap convention.

For $n\geq3$, the nearest [pole](../../../../../pole.md) to the real axis is $\vartheta=ia$. It is simple and comes from the first factor. In the crossed, or [t-channel](../../../../../scattering-t-channel.md), the [momentum](../../../../../momentum.md) carried between the external particles is their difference. With the $+,-$ metric its invariant is

$$
t=m_2^2+m_1^2-2m_2m_1\cosh\vartheta.
$$

At the [pole](../../../../../pole.md), substitute the [breather](../../../../../breather.md) [masses](../../../../../mass.md):

$$
\begin{aligned}
t&=4M^2\left[\sin^2(2a)+\sin^2a-2\sin(2a)\sin a\cos a\right]\\
&=4M^2\sin^2a=\boxed{m_1^2}.
\end{aligned}
$$

The trigonometric identity is applied with angles $2a$ and $a$. Thus the exchanged one-particle state is **the lightest [breather](../../../../../breather.md) $\mathcal B_1$**, on its [mass shell](../../../../../mass-shell.md). This is [crossed-channel lightest-breather exchange](../../../../../crossed-channel-lightest-breather-exchange.md). The external momenta at a bound-state [pole](../../../../../pole.md) are analytically continued; [on shell](../../../../../on-shell.md) here means the invariant [mass](../../../../../mass.md) relation and conservation of the continued energy-momentum, not a [pole](../../../../../pole.md) at real physical [rapidity](../../../../../rapidity.md). At $n=3$ the more distant central factor has a [double pole](../../../../../double-pole.md), but the nearest $ia$ [pole](../../../../../pole.md) and its $\mathcal B_1$ interpretation remain unchanged.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
