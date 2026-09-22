<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Normalize both leading coefficients to one. For the [indicial root](../../../../indicial-root.md) $a=1/2$, the [recurrence relation](../../../../recurrence-relation.md) from part (b) gives

$$
c_{2k}=\frac{(-1)^k}{(2k+1)!},\qquad c_{2k+1}=0.
$$

Recognizing the [Taylor series](../../../../taylor-series.md) of the [sine](../../../../sine.md) gives the first [Frobenius solution](../../../../frobenius-solution.md)

$$
\boxed{y_+(x)=x^{1/2}\sum_{k=0}^\infty\frac{(-1)^kx^{2k}}{(2k+1)!}
=\frac{\sin x}{\sqrt x}.}
$$

For the smaller [indicial root](../../../../indicial-root.md) $-1/2$, $n(n-1)d_n=-d_{n-2}$. The equation at $n=1$ is $0=0$; choose the free coefficient $d_1=0$ to avoid adding the first [Frobenius solution](../../../../frobenius-solution.md). The remaining coefficients are

$$
d_{2k}=\frac{(-1)^k}{(2k)!},\qquad d_{2k+1}=0.
$$

Thus the [Taylor series](../../../../taylor-series.md) of the [cosine](../../../../cosine.md) gives

$$
\boxed{y_-(x)=x^{-1/2}\sum_{k=0}^\infty\frac{(-1)^kx^{2k}}{(2k)!}
=\frac{\cos x}{\sqrt x}.}
$$

Their leading terms are $x^{1/2}$ and $x^{-1/2}$, as required for Case IIIb. A direct check uses $y=x^{-1/2}u$: the [differential equation](../../../../differential-equation-split.md) becomes $x^{3/2}(u''+u)=0$, so these two functions solve it on $x>0$. Their [Wronskian](../../../../wronskian.md) is $-1/x\ne0$, proving [linear independence](../../../../linear-independence.md). The [general solution](../../../../general-solution.md) is $(C_1\sin x+C_2\cos x)/\sqrt x$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the differential equations 2 course of the University of Oxford](../../../split.md)
5. [Differential equations 2 course of the University of Oxford](../../../../differential-equations-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
