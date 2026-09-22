<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $L=-(1-x^2)D^2+xD$, so $Ly_n=n^2y_n$ and the forced equation is $(\gamma^2-L)Z=e^{\varepsilon x}$. The small-parameter [Taylor expansion](../../../../../../taylor-expansion.md) of the forcing is

$$
e^{\varepsilon x}=1+\varepsilon x+\frac{\varepsilon^2x^2}{2}+O(\varepsilon^3)
=y_0+\varepsilon y_1+\frac{\varepsilon^2}{4}(y_0+y_2)+O(\varepsilon^3).
$$

Each [Chebyshev polynomial](../../../../../../chebyshev-polynomial.md) can be inverted separately under $\gamma^2-L$. None of the required denominators vanishes because $\gamma$ is a real noninteger. Thus the [regular solution of a forced Chebyshev equation](../../../../../../regular-solution-of-a-forced-chebyshev-equation.md) has

$$
\boxed{A=\frac{y_0}{\gamma^2},\qquad
B=\frac{y_1}{\gamma^2-1},\qquad
C=\frac{y_0}{4\gamma^2}+\frac{y_2}{4(\gamma^2-4)}}.
$$

Here we select the same regular endpoint domain as in part (a), with finite function values and finite endpoint [derivatives](../../../../../../derivative.md). This qualification is needed: the printed forced equation alone does not state endpoint conditions. Without this selection one can add $c_1\cos(\gamma\arccos x)+c_2\sin(\gamma\arccos x)$, which remain finite but generally have singular endpoint [derivatives](../../../../../../derivative.md). With $x=\cos\theta$, regularity gives $Z_\theta(0)=Z_\theta(\pi)=0$; the corresponding homogeneous equation has only the zero solution for noninteger $\gamma$. This makes the displayed expansion unique.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
