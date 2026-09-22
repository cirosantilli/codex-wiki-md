<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\tau=t-t'$ and $\Omega=\sqrt{K^2-b^2}>0$. Because $|e^{-i(u+iv)\tau}|=e^{v\tau}$, close below for $\tau>0$ and above for $\tau<0$. The lower closure is clockwise. The two [residues](../../../../../residue.md) sum to $i e^{b\tau}\sin(\Omega\tau)/\Omega$. Hence, for nonzero $b$,

$$
\boxed{G(\tau)=
\begin{cases}
-e^{b\tau}\sin(\Omega\tau)H(-\tau)/\Omega,&b>0,\\
 e^{b\tau}\sin(\Omega\tau)H(\tau)/\Omega,&b<0.
\end{cases}}
$$

In particular, **the printed sign with $e\gamma>0$ gives zero for $t>t'$ and an [advanced Green function](../../../../../advanced-green-function.md) for $t<t'$**. Reversing that sign puts the [poles](../../../../../pole.md) below and gives a [retarded Green function](../../../../../retarded-green-function.md). Both solutions have the unit [derivative](../../../../../derivative.md) jump required by $(\partial_\tau^2-2b\partial_\tau+K^2)G=\delta(\tau)$. If $b=0$, the bare integral has real-axis [poles](../../../../../pole.md) and requires an additional contour prescription; a unique retarded or advanced answer cannot be inferred without one.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the theoretical physics I course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics I course of the University of Cambridge](../../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
