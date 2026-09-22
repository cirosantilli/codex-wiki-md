<h1 id="13b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The first mode remains the solution from part (b). The applied force excites only the third mode, so

$$
y(x,t)=Ate^{-kt}\sin\frac{\pi x}{l}
+q_3(t)\sin\frac{3\pi x}{l},
$$

where, using $\pi c/l=k$,

$$
q_3''+2kq_3'+9k^2q_3=\alpha\cos kt,
\qquad q_3(0)=q_3'(0)=0.
$$

A particular solution is

$$
q_{3,p}(t)=\frac{\alpha}{34k^2}(4\cos kt+\sin kt).
$$

Adding the decaying complementary solution and imposing the initial conditions gives

$$
\boxed{
q_3(t)=\frac{\alpha}{34k^2}
\left[
4\cos kt+\sin kt
-e^{-kt}\left(
4\cos(2\sqrt2kt)
+\frac5{\sqrt2}\sin(2\sqrt2kt)
\right)
\right]}.
$$

As $t\to\infty$, all transients decay but the driven third-mode oscillation remains. The string approaches a periodic [steady-state response](../../../../../../steady-state-response.md), rather than coming to rest.

With gravity omitted, its mechanical energy is

$$
E=\frac{\mu}{2}\int_0^l
\left(y_t^2+c^2y_x^2\right)dx.
$$

Writing $s=\alpha/(34k^2)$ and letting $t\to\infty$ gives

$$
\boxed{
E_\infty(t)
=\frac{\mu l\alpha^2}{4624k^2}
\left[
25\sin^2kt+145\cos^2kt
+64\sin kt\cos kt
\right]}.
$$

The limiting energy is periodic because the external force continually supplies the energy dissipated by drag.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [13B](../../13b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
