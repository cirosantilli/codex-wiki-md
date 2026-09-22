<h1 id="d/d4/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiating the integral representation gives

$$
J_0'(t)=-\frac2\pi\int_0^{\pi/2}\cos x\sin(t\cos x)\,dx,
\qquad
J_0''(t)+J_0(t)=\frac2\pi\int_0^{\pi/2}\sin^2x\cos(t\cos x)\,dx.
$$

Now integrate the derivative

$$
\frac d{dx}\big(\sin x\sin(t\cos x)\big)
=\cos x\sin(t\cos x)-t\sin^2x\cos(t\cos x).
$$

The boundary terms vanish at both endpoints. Consequently $J_0'(t)=-t(J_0''(t)+J_0(t))$, proving

$$
\boxed{tJ_0''(t)+J_0'(t)+tJ_0(t)=0.}
$$

The identity includes $t=0$, where it reads $J_0'(0)=0$.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [1](../../1.md)
3. [D4](../../../d4.md)
4. [D](../../../../d.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
