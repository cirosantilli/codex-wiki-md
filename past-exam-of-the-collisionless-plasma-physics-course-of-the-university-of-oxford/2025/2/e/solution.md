<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The real [Airy function](../../../../airy-function.md) asymptotics used for the [Airy turning-point connection formula](../../../../airy-turning-point-connection-formula.md) are, for $z,s\to+\infty$,

$$
\begin{aligned}
\operatorname{Ai}(z)&\sim\frac{z^{-1/4}}{2\sqrt\pi}e^{-2z^{3/2}/3},&
\operatorname{Bi}(z)&\sim\frac{z^{-1/4}}{\sqrt\pi}e^{2z^{3/2}/3},\\
\operatorname{Ai}(-s)&\sim\frac{s^{-1/4}}{\sqrt\pi}\sin(2s^{3/2}/3+\pi/4),&
\operatorname{Bi}(-s)&\sim\frac{s^{-1/4}}{\sqrt\pi}\cos(2s^{3/2}/3+\pi/4).
\end{aligned}
$$

These real-axis asymptotics fix both normalization and phase.[Equations 9.7.5, 9.7.7, 9.7.9 and 9.7.11; leading terms for positive real argument](../../../../airy-function-asymptotics-in-the-digital-library-of-mathematical-functions.md) Near $a$, $I\sim2z^{3/2}/3$, $\Phi\sim2(-z)^{3/2}/3$, and $\kappa^{-1/2}\sim\ell^{1/2}z^{-1/4}$. Matching to the constants of [c](../c.md) gives $C_A=2\sqrt\pi\ell^{1/2}D$ and $C_B=\sqrt\pi\ell^{1/2}G$. Therefore

$$
\boxed{\frac{D e^{-I}+G e^I}{\sqrt\kappa}
\quad\longleftrightarrow\quad
\frac{2D\cos(\Phi-\pi/4)-G\sin(\Phi-\pi/4)}{\sqrt{k_1}}.}
$$

In particular, the decaying component matches the cosine with the requested $-\pi/4$ shift, with a factor **two** in its oscillatory coefficient. The growing component matches a sine with the indicated minus sign. Expanding into travelling [waves](../../../../wave-split.md) gives

$$
\boxed{A_{\rm in}=D-\frac{iG}{2},\qquad A_{\rm r}=D+\frac{iG}{2}.}
$$

The factor two is essential when converting the real oscillatory components to incident and reflected travelling [waves](../../../../wave-split.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
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
