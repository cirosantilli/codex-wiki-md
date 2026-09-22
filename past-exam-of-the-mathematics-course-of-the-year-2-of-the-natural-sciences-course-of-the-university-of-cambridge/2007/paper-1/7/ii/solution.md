<h1 id="7/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Multiplying by $y$ and integrating with the zero endpoint values first gives $\lambda\int_1^by^2dx/x=\int_1^bx(y')^2dx>0$ for a nonzero real [eigenfunction](../../../../../eigenfunction.md); hence $\lambda>0$. Using the printed [change of variables](../../../../../change-of-variables-formula.md) $\xi=\lambda\ln x$, write $y(x)=Y(\xi)$. Then $(xy')'=\lambda^2Y_{\xi\xi}/x$, so $Y_{\xi\xi}+Y/\lambda=0$. The first endpoint gives $Y=A\sin(\xi/\sqrt\lambda)$, and the other gives $\sin(\sqrt\lambda\ln b)=0$. Thus

$$
\boxed{\lambda_n=\left(\frac{n\pi}{\ln b}\right)^2,\qquad y_n(x)=A_n\sin\left(\frac{n\pi\ln x}{\ln b}\right),\quad n=1,2,\ldots.}
$$

This is the [logarithmic change of variable in a Sturm-Liouville problem](../../../../../logarithmic-change-of-variable-in-a-sturm-liouville-problem.md). The measure $dx/x=d(\ln x)$ gives squared [weighted norm](../../../../../weighted-norm.md) $A_n^2\ln b/2$, so an orthonormal choice is $A_n=\sqrt{2/\ln b}$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
