<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $I_1$, the [change of variables](../../../../../../../change-of-variables-formula.md) $t=x^2/\theta$ gives

$$
\boxed{I_1=\int_0^\infty e^{-t}\,dt=1.}
$$

For $k\geq1$, use $d(e^{-x^2/\theta})=-(2x/\theta)e^{-x^2/\theta}\,dx$ and [integration by parts](../../../../../../../integration-by-parts.md):

$$
\begin{aligned}
I_{k+2}&=-\int_0^\infty x^{k+1}\,d(e^{-x^2/\theta})\\
&=-\left[x^{k+1}e^{-x^2/\theta}\right]_0^\infty+(k+1)\int_0^\infty x^ke^{-x^2/\theta}\,dx\\
&=\boxed{\frac{(k+1)\theta}{2}I_k.}
\end{aligned}
$$

The boundary term vanishes: $x^{k+1}\to0$ at zero, and the [exponential decay](../../../../../../../exponential-decay.md) dominates the power at infinity. These estimates also establish convergence of the [improper integrals](../../../../../../../improper-integral.md) used above.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
