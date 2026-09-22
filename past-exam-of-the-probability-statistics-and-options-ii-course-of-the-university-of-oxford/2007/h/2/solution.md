<h1 id="h/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $q=(x,X)^{\mathsf T}$, $M=\begin{pmatrix}a&b\\b&c\end{pmatrix}$ and $K=\begin{pmatrix}\alpha&\beta\\\beta&\gamma\end{pmatrix}$. The [Euler-Lagrange equations](../../../../euler-lagrange-equation.md) give $M\ddot q+Kq=0$. A [normal mode](../../../../normal-mode.md) is a motion $q=v\cos(\omega t+\varphi)$ with fixed nonzero [vector](../../../../vector.md) $v$; its [normal frequency](../../../../eigenfrequency.md) is $\omega>0$. Substitution gives $(K-\omega^2M)v=0$. Thus the squared [normal frequencies](../../../../eigenfrequency.md) are the assumed positive distinct roots of

$$
(ac-b^2)\lambda^2-(\alpha c+\gamma a-2\beta b)\lambda+(\alpha\gamma-\beta^2)=0.
$$

For either root, solve the associated two linear equations for the mode ratio.

For the rods, the small angles are $\theta=x/a$ and $\phi=(X-x)/(2a)$. The first rod has [kinetic energy](../../../../kinetic-energy.md) $m\dot x^2/6$. The second rod's center has horizontal [velocity](../../../../velocity.md) $(\dot x+\dot X)/2$ and its [angular velocity](../../../../angular-velocity.md) is $(\dot X-\dot x)/(2a)$. Its center-of-mass [moment of inertia](../../../../moment-of-inertia.md) is $2ma^2/3$, giving

$$
T_2=\frac m4(\dot x+\dot X)^2+\frac m{12}(\dot X-\dot x)^2.
$$

Adding these [kinetic energies](../../../../kinetic-energy.md) gives $T=m(3\dot x^2+2\dot x\dot X+2\dot X^2)/6$. The first center rises by $a\theta^2/4$, and the second by $a\theta^2/2+a\phi^2/2$. Multiplying by the respective masses and $g$ gives

$$
V=\frac{mg}{4a}\bigl[5x^2+(X-x)^2\bigr]
=\frac{mg}{4a}(6x^2-2xX+X^2).
$$

Therefore the stated [Lagrangian](../../../../lagrangian.md) is $T-V$.

Set $\mu=2a\omega^2/(3g)$. The mode equation is

$$
\det\left[\begin{pmatrix}6&-1\\-1&1\end{pmatrix}
-\mu\begin{pmatrix}3&1\\1&2\end{pmatrix}\right]
=5\mu^2-17\mu+5=0.
$$

Hence

$$
\boxed{\omega_\pm^2=\frac{3g}{20a}(17\pm3\sqrt{21}).}
$$

The mode ratio is $r=X/x=(6-3\mu)/(1+\mu)$, so the ratio of the rods' angles is $\phi/\theta=(r-1)/2=(5-4\mu)/[2(1+\mu)]$. It is positive for $\mu_-=(17-3\sqrt{21})/10$ and negative for $\mu_+=(17+3\sqrt{21})/10$. Thus the lower-frequency [normal mode](../../../../normal-mode.md) has the rods **in phase**, and the higher-frequency [normal mode](../../../../normal-mode.md) has them **out of phase**.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [H](../../h.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
