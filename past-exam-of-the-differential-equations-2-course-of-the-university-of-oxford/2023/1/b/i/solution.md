<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Set $a=\pi/2$. To construct the [Green's function](../../../../../green-s-function-split.md) from a [Dirac delta function](../../../../../dirac-delta-function.md), require $\mathcal L_xg(x,\xi)=\delta(x-\xi)$ and zero endpoint values. Away from $x=\xi$, the [homogeneous solutions](../../../../../homogeneous-solution.md) satisfying the left and right [boundary conditions](../../../../../boundary-condition.md) are respectively

$$
u(x)=e^{-x}\sin x,\qquad v(x)=e^{-x}\cos x.
$$

Write $g=A(\xi)u(x)$ for $x<\xi$ and $g=B(\xi)v(x)$ for $x>\xi$. A discontinuity in $g$ would generate a derivative of the [Dirac delta function](../../../../../dirac-delta-function.md), which is absent from the desired equation. Thus $g$ is continuous. Integrating that equation through $\xi$ then gives the [jump condition](../../../../../jump-condition.md)

$$
g_x(\xi^+,\xi)-g_x(\xi^-,\xi)=1.
$$

The resulting two equations are $Au(\xi)=Bv(\xi)$ and $Bv'(\xi)-Au'(\xi)=1$. Since the [Wronskian](../../../../../wronskian.md) $uv'-u'v=-e^{-2\xi}$, they give

$$
\boxed{g(x,\xi)=-e^{\xi-x}
\begin{cases}
\sin x\cos\xi,&0\leq x\leq\xi,\\
\sin\xi\cos x,&\xi\leq x\leq\pi/2.
\end{cases}}
$$

Both endpoint values vanish. At $x=\xi$, subtracting the two first [derivatives](../../../../../derivative.md) gives $\sin^2\xi+\cos^2\xi=1$, verifying the sign and normalization of the [Dirac delta function](../../../../../dirac-delta-function.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
