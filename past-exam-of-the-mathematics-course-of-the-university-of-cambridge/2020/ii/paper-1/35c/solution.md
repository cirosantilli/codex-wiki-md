<h1 id="35c/solution">Solution</h1>

↑ **Parent:** [35C](../35c.md)

In the [Parity basis of a one-dimensional S-matrix](../../../../../parity-basis-of-a-one-dimensional-s-matrix.md), parity acts as $\mathcal P=\operatorname{diag}(1,-1)$. [Parity](../../../../../parity.md) invariance requires

$$
[S,\mathcal P]=0,
$$

and therefore

$$
S_{+-}=S_{-+}=0.
$$

Independently, [unitarity](../../../../../unitary-operator.md) gives

$$
|S_{++}|^2+|S_{-+}|^2=1,
\qquad
|S_{--}|^2+|S_{+-}|^2=1,
\qquad
S_{++}^*S_{+-}+S_{-+}^*S_{--}=0.
$$

Combining parity and unitarity leaves two phases,

$$
\boxed{S=\operatorname{diag}(e^{2i\delta_+},e^{2i\delta_-})}.
$$

For the [symmetric double-delta potential](../../../../../symmetric-double-delta-potential.md), consider the odd channel on $x\geq0$. Choose the asymptotic convention

$$
\psi(x)=e^{-ikx}-S_{--}e^{ikx},\qquad x>a,
$$

and write $psi(x)=C\sin(kx)$ for $0<x<a$; the sine enforces odd [parity](../../../../../parity.md) at the origin. Continuity and the [delta potential](../../../../../delta-potential.md) derivative jump at $x=a$ give

$$
C\sin(ka)=e^{-ika}-S_{--}e^{ika},
$$



$$
-ik e^{-ika}-ikS_{--}e^{ika}-Ck\cos(ka)
=U_0C\sin(ka).
$$

Eliminating $C$ yields the [Odd-parity S-matrix of a symmetric double-delta potential](../../../../../odd-parity-s-matrix-of-a-symmetric-double-delta-potential.md)

$$
S_{--}=e^{-2ika}
\frac{k e^{ika}+U_0\sin(ka)}
{k e^{-ika}+U_0\sin(ka)}.
$$

Using $2i\sin(ka)=e^{ika}-e^{-ika}$ rewrites this as the requested expression

$$
\boxed{
S_{--}=e^{-i2ka}
\frac{(2k-iU_0)e^{ika}+iU_0e^{-ika}}
{(2k+iU_0)e^{-ika}-iU_0e^{ika}}.
}
$$

For real $k$, the two factors in the ratio are complex conjugates, directly confirming $|S_{--}|=1$.

A [bound state](../../../../../bound-state-poles-of-a-partial-wave-s-matrix.md) occurs at a pole $k=i\kappa$, $kappa>0$. Setting the denominator to zero gives

$$
\kappa e^{\kappa a}+U_0\sinh(\kappa a)=0,
$$

or

$$
\boxed{2\kappa=-U_0(1-e^{-2\kappa a}).}
$$

For $U_0<0$, write $g=-U_0>0$. The right-hand side $g(1-e^{-2\kappa a})$ is increasing and concave, starts at zero with slope $2ga$, and approaches $g$, whereas the left-hand side is the straight line $2\kappa$. A positive intersection therefore exists exactly when

$$
\boxed{-U_0a>1.}
$$

This is the [odd bound state of a symmetric double-delta potential](../../../../../odd-bound-state-of-a-symmetric-double-delta-potential.md); equality is its zero-energy threshold.

For $U_0>0$, analytically continue the same pole equation into the lower half of the complex $k$-plane. Put

$$
z=ka,qquad G=U_0a.
$$

It becomes

$$
z e^{-iz}+G\sin z=0.
$$

When $G\gg1$, the lowest odd mode lies near the hard-wall value $z=\pi$. Writing $z=\pi+\eta$ and expanding gives

$$
(\pi+\eta)e^{-i\eta}+G\eta=0,
$$

so

$$
\eta=-\frac\pi G+\frac{\pi-i\pi^2}{G^2}+O(G^{-3}).
$$

In particular, the [odd resonance of a strongly repulsive symmetric double-delta potential](../../../../../odd-resonance-of-a-strongly-repulsive-symmetric-double-delta-potential.md) has

$$
\boxed{
k_R=\frac\pi a\left(1-\frac1{U_0a}+O((U_0a)^{-2})\right),
\qquad
k_I=-\frac{\pi^2}{U_0^2a^3}+O((U_0a)^{-3}/a).
}
$$

The negative imaginary part identifies a decaying [scattering resonance](../../../../../scattering-resonance.md). If

$$
E=\frac{\hbar^2k^2}{2m}=E_R-\frac{i\Gamma}{2},
$$

then, to leading nonzero order,

$$
\Gamma=-2\operatorname{Im}E
=\frac{2\hbar^2\pi^3}{mU_0^2a^4}.
$$

Its time-dependent amplitude is proportional to

$$
e^{-iEt/\hbar}=e^{-iE_Rt/\hbar}e^{-\Gamma t/(2\hbar)},
$$

so its survival probability decays as $e^{-\Gamma t/\hbar}$ and its lifetime is

$$
\boxed{\tau=\frac\hbar\Gamma
=\frac{mU_0^2a^4}{2\hbar\pi^3}.}
$$

Physically, this is the lowest odd standing wave trapped for a long time between two strong repulsive barriers and leaking out by [quantum tunnelling](../../../../../quantum-tunnelling.md).

## ↑ Ancestors (10)

1. [35C](../35c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
