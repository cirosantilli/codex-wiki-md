<h1 id="7/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The displacement directions specified at release give $x(0)=(-x_0,x_0)^T$. Let $\Delta r=r_--r_+=2D/m_2>0$. By [initial-data decomposition into two normal modes](../../../../../initial-data-decomposition-into-two-normal-modes.md), write $x(0)=c_-v_-+c_+v_+$. Solving the two coordinate equations gives

$$
c_-=\frac{x_0(1+r_+)}{\Delta r},\qquad c_+=-\frac{x_0(1+r_-)}{\Delta r}.
$$

Zero initial velocities remove the sine terms, so

$$
\boxed{x(t)=\frac{x_0}{\Delta r}\left[(1+r_+)v_-\cos(\omega_-t)-(1+r_-)v_+\cos(\omega_+t)\right].}
$$

In components,

$$
\boxed{\begin{aligned}
x_1(t)&=\frac{x_0}{\Delta r}[(1+r_+)\cos(\omega_-t)-(1+r_-)\cos(\omega_+t)],\\
x_2(t)&=\frac{x_0}{\Delta r}[r_-(1+r_+)\cos(\omega_-t)-r_+(1+r_-)\cos(\omega_+t)].
\end{aligned}}
$$

Substitution at zero gives $x_1=-x_0$, $x_2=x_0$, and both derivatives vanish. For unequal masses both [normal modes](../../../../../normal-mode.md) are generally present. When $m_1=m_2=m$, $r_-=1$, $r_+=-1$, so only the higher mode survives: $x_1=-x_0\cos(\sqrt{3k/m}\,t)$ and $x_2=x_0\cos(\sqrt{3k/m}\,t)$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [7](../../7.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
