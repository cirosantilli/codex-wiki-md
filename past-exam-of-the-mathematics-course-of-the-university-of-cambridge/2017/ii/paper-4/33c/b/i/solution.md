<h1 id="33c/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the odd channel, solve on $x>0$ with $\psi(0)=0$. Inside $0<x<a$, write $\psi=C\sin(kx)$; outside write $\psi=e^{-ikx}-S_{--}e^{ikx}$, respecting the outgoing odd-channel minus sign. [Continuity](../../../../../../../continuous-function.md) at $a$ and the delta-potential [derivative](../../../../../../../derivative.md) jump are

$$
C\sin(ka)=e^{-ika}-S_{--}e^{ika},\qquad
-ik(e^{-ika}+S_{--}e^{ika})-Ck\cos(ka)=U_0(e^{-ika}-S_{--}e^{ika}).
$$

Eliminating $C$ yields

$$
\boxed{S_{--}(k)=e^{-2ika}\frac{(2k-iU_0)e^{ika}+iU_0e^{-ika}}{(2k+iU_0)e^{-ika}-iU_0e^{ika}}.}
$$

The equations remain valid when $\sin(ka)=0$ by taking the limiting value, rather than dividing blindly. For real $k,U_0$, numerator and denominator inside the fraction are complex conjugates and the prefactor has unit modulus. Thus $|S_{--}|^2=1$. This is conservation of flux in the odd [parity](../../../../../../../parity.md) channel: the real potential causes only a phase shift there, not absorption. It does not assert unit left-to-right transmission in the usual incident-from-one-side basis.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [33C](../../../33c.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
