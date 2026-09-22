<h1 id="s18/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $L_0\psi=-U\psi$ and use the outgoing inverse of $L_0$. Adding the homogeneous incoming wave yields

$$
\psi=e^{ikx}-\frac{im}{k\hbar^2}\int e^{ik|x-x'|}U(x')\psi(x')\,dx'.
$$

For the attractive delta potential, let $\eta=m\alpha/(k\hbar^2)$. The equation reduces to $\psi(x)=e^{ikx}+i\eta e^{ik|x|}\psi(0)$ and $\psi(0)=1/(1-i\eta)$. Separating the two half-lines gives

$$
\boxed{t=\frac1{1-i\eta},\qquad r=\frac{i\eta}{1-i\eta},\qquad
\psi=\begin{cases}e^{ikx}+re^{-ikx},&x<0,\\te^{ikx},&x>0.\end{cases}}
$$

Both sides have the same [group velocity](../../../../../group-velocity.md), so

$$
\boxed{T=\frac1{1+\eta^2},\qquad R=\frac{\eta^2}{1+\eta^2},\qquad T+R=1.}
$$

The same amplitudes satisfy continuity and the exact delta-potential [derivative](../../../../../derivative.md) jump $\psi'(0^+)-\psi'(0^-)=-2m\alpha\psi(0)/\hbar^2$, providing an independent local check on the sign.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [S18](../../../s18.md)
4. [2018](../../../../2018-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
