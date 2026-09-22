<h1 id="5b/solution">Solution</h1>

↑ **Parent:** [5B](../5b.md)

Set $u(r,\theta)=R(r)\Theta(\theta)$. Periodicity and [separation of variables](../../../../../separation-of-variables.md) give the angular modes $1$, $\cos n\theta$, and $\sin n\theta$. The radial equation is

$$
r^2R''+rR'-n^2R=0,
$$

whose solutions are $r^{\pm n}$ for $n\geq1$; the zero mode has solutions $1$ and $\log r$. Thus a general real harmonic [function](../../../../../function-split.md) on the annulus is

$$
\begin{aligned}
u(r,\theta)={}&A_0+B_0\log r\\
&+\sum_{n=1}^{\infty}
\left(A_nr^n+B_nr^{-n}\right)\cos n\theta\\
&+\sum_{n=1}^{\infty}
\left(C_nr^n+D_nr^{-n}\right)\sin n\theta.
\end{aligned}
$$

The boundary data contain only the $n=2$ cosine mode, so write

$$
u=(Ar^2+Br^{-2})\cos2\theta.
$$

The condition at $r=a$ gives $B=-Aa^4$, and the condition at $r=b$ fixes $A$. The [Dirichlet problem on an annulus for one Fourier mode](../../../../../dirichlet-problem-on-an-annulus-for-one-fourier-mode.md) therefore has solution

$$
\boxed{
u(r,\theta)=
\frac{b^2(r^4-a^4)}{r^2(b^4-a^4)}\cos2\theta}.
$$

## ↑ Ancestors (10)

1. [5B](../5b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
