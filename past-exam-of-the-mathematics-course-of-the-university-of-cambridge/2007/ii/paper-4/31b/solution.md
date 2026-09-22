<h1 id="31b/solution">Solution</h1>

↑ **Parent:** [31B](../31b.md)

Away from the turning points, the [Liouville–Green approximation](../../../../../wkb-approximation.md) gives in the allowed region

$$
\psi\sim q^{-1/4}\left[A\cos\left(\lambda\int_a^x\sqrt q\,ds\right)
+B\sin\left(\lambda\int_a^x\sqrt q\,ds\right)\right].
$$

The bound-state condition discards the growing exponential in each forbidden region, leaving

$$
\psi_L\sim C_L(-q)^{-1/4}\exp\left[-\lambda\int_x^a\sqrt{-q}\,ds\right],\qquad
\psi_R\sim C_R(-q)^{-1/4}\exp\left[-\lambda\int_b^x\sqrt{-q}\,ds\right].
$$

These approximations require variation slow compared with the local wavelength, and must be replaced near $a,b$ by Airy approximations.

Near $a$, set $z=-\lambda^{2/3}q'(a)^{1/3}(x-a)$. The local differential equation becomes $\psi_{zz}-z\psi=0$. Decay on the left selects [Airy function](../../../../../airy-function.md) $\operatorname{Ai}(z)$ rather than its growing companion. Comparing the supplied asymptotics across the turning point yields

$$
\psi\sim2C_Lq^{-1/4}\cos\left(S_a(x)-\frac\pi4\right),
\qquad S_a(x)=\lambda\int_a^x\sqrt q\,ds.
$$

At $b$, use $z=\lambda^{2/3}[-q'(b)]^{1/3}(x-b)$; decay on the right similarly yields $2C_Rq^{-1/4}\cos(S_b(x)-\pi/4)$, where $S_b=\lambda\int_x^b\sqrt q\,ds$. Let $J=S_a+S_b=\lambda\int_a^b\sqrt q\,ds$. The left expression has equal cosine and sine coefficients in the variable $S_a$; the right expression has those coefficients proportional to $\cos(J-\pi/4)$ and $\sin(J-\pi/4)$. They can describe the same nonzero wave only when $J-\pi/4=\pi/4+n\pi$. Therefore the [WKB quantization condition](../../../../../wkb-quantization-condition.md) is

$$
\boxed{\lambda\int_a^b\sqrt{q(x)}\,dx=(n+\tfrac12)\pi,
\qquad n=0,1,2,\ldots.}
$$

The two simple turning points contribute the two quarter-phase shifts, giving the half-integer correction.

## ↑ Ancestors (10)

1. [31B](../31b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
