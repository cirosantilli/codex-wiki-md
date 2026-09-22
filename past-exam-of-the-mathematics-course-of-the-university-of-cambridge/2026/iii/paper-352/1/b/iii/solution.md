<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

In either half-plane, let $U_\infty$ denote its far-field value. Multiplying the ODE by $U'$ and integrating from the far field gives

$$
HK\frac n{n+1}|U'|^{n+1}
=\frac\mu{2h}(U-U_\infty)^2.
$$

Since the profile decreases,

$$
\boxed{U'=-A|U-U_\infty|^{2/(n+1)}},
\qquad
A=\left[\frac{\mu(n+1)}{2hHKn}\right]^{1/(n+1)}.
$$

Continuity of $U'$ at $y=0$ gives

$$
U(0)=U_0=\frac{U_-+U_+}{2}.
$$

For $n=1$, let $\ell=A^{-1}=\sqrt{hHK/\mu}$ and $\Delta U=U_--U_+$. Then

$$
\boxed{
U(y)=
\begin{cases}
U_--\dfrac{\Delta U}{2}e^{y/\ell},&y<0,\\
U_++\dfrac{\Delta U}{2}e^{-y/\ell},&y>0.
\end{cases}}
$$

The Newtonian disturbance therefore has exponential tails.

For $n<1$ and $y>0$, put $W=U-U_+$. Integration gives

$$
\boxed{U(y)=U_++
\left[
(U_0-U_+)^{-(1-n)/(n+1)}
+\frac{1-n}{n+1}Ay
\right]^{-(n+1)/(1-n)}}.
$$

The corresponding expression on $y<0$ follows by reflection about $(0,U_0)$. A [shear thinning](../../../../../../../shear-thinning.md) power-law material has algebraic rather than exponential margin tails. Measurements of how rapidly an ice-stream speed approaches its far-field values could therefore distinguish an approximately Newtonian rheology from power-law shear thinning and estimate $n$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 352](../../../../paper-352-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
