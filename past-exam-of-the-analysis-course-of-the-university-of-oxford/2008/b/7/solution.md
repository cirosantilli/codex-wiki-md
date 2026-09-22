<h1 id="b/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

With the classical real coefficients

$$
a_j=\frac1\pi\int_{-\pi}^\pi f(x)\cos(jx)dx,\qquad b_j=\frac1\pi\int_{-\pi}^\pi f(x)\sin(jx)dx,
$$

the partial sum is $s_n^f=a_0/2+\sum_{j=1}^n(a_j\cos jx+b_j\sin jx)$. It is the [orthogonal projection](../../../../orthogonal-projection.md) onto the first trigonometric modes. [Completeness](../../../../completeness.md) of the trigonometric [orthonormal](../../../../orthonormal-set.md) system therefore gives $\|s_n^f-f\|_2\to0$.

For $f\in C^1$ periodic, [integration by parts](../../../../integration-by-parts.md) has zero endpoint terms and gives $a_j(f')=jb_j(f)$, $b_j(f')=-ja_j(f)$, and $a_0(f')=0$. Thus

$$
\boxed{s_n^{f'}(x)=\sum_{j=1}^n[jb_j(f)\cos jx-ja_j(f)\sin jx]=(s_n^f)'(x).}
$$

For periodic $C^2$ functions, another [integration by parts](../../../../integration-by-parts.md) gives $a_j(f)=-a_j(f'')/j^2$ and $b_j(f)=-b_j(f'')/j^2$. Riemann-Lebesgue makes the numerator sequences tend to zero, in particular bounded. The [Weierstrass M-test](../../../../weierstrass-m-test.md) and $\sum j^{-2}<\infty$ prove absolute and [uniform convergence](../../../../uniform-convergence.md). The resulting [continuous](../../../../continuous-function.md) sum agrees with $f$ in $L^2$ by the first result. Two [continuous](../../../../continuous-function.md) functions equal almost everywhere are equal everywhere, so the pointwise sum is $f$ for every real $x$.

For the [polynomial](../../../../polynomial-split.md) example the periodic extension is $C^2$: the function, its first [derivative](../../../../derivative.md) and its second [derivative](../../../../derivative.md) match at the endpoints. It is even, so all sine coefficients vanish. Direct integration gives

$$
\frac{a_0}{2}=\frac{7\pi^4}{15},\qquad a_j=\frac{48(-1)^j}{j^4}\quad(j\geq1).
$$

For example, [integration by parts](../../../../integration-by-parts.md) gives $\int_0^\pi x^2\cos(jx)dx=2\pi(-1)^j/j^2$ and $\int_0^\pi x^4\cos(jx)dx=4\pi^3(-1)^j/j^2-24\pi(-1)^j/j^4$, from which the cancellation of the $j^{-2}$ terms follows. Therefore

$$
\boxed{f(x)=\frac{7\pi^4}{15}+48\sum_{j=1}^\infty\frac{(-1)^j\cos(jx)}{j^4}.}
$$

At $x=0$, the left side vanishes, yielding

$$
\boxed{\sum_{j=1}^\infty\frac{(-1)^{j+1}}{j^4}=\frac{7\pi^4}{720}.}
$$

## ↑ Ancestors (12)

1. [7](../7.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
