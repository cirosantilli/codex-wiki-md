<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use $c_j=(\gamma_j^A+i\gamma_j^B)/2$ and $c_j^\dagger=(\gamma_j^A-i\gamma_j^B)/2$. Moving operators from different modes past one another introduces a minus sign. Direct expansion gives

$$
\begin{aligned}
c_1^\dagger c_2+c_2^\dagger c_1
&=\frac i2(\gamma_1^A\gamma_2^B-\gamma_1^B\gamma_2^A),\\
c_1^\dagger c_2^\dagger+c_2c_1
&=-\frac i2(\gamma_1^A\gamma_2^B+\gamma_1^B\gamma_2^A).
\end{aligned}
$$

Thus, for real hopping and pairing parameters,

$$
H=\frac i2\left[(\Delta-t)\gamma_1^A\gamma_2^B+(t+\Delta)\gamma_1^B\gamma_2^A\right].
$$

At $\Delta=t\ne0$ this becomes

$$
\boxed{H=it\gamma_1^B\gamma_2^A}.
$$

Use $\tau$ for time to distinguish it from the hopping amplitude $t$. Each unused Majorana operator anticommutes with both factors in $H$, so commuting it through their product gives two minus signs. Hence $[H,\gamma_1^A]=[H,\gamma_2^B]=0$. The [Heisenberg picture](../../../../heisenberg-picture.md) equation $dO/d\tau=(i/\hbar)[H,O]$ therefore gives

$$
\boxed{\gamma_1^A(\tau)=\gamma_1^A(0),\qquad \gamma_2^B(\tau)=\gamma_2^B(0)}.
$$

These are the two uncoupled [Majorana zero modes](../../../../majorana-zero-mode.md).

## ↑ Ancestors (14)

1. [C](../c.md)
2. [1](../../1.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the theoretical physics II course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics II course of the University of Cambridge](../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
