<h1 id="5/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take $0\leq r<R$. At the point $r$, the [power series](../../../../../../../power-series.md) has [absolute convergence](../../../../../../../absolute-convergence.md), so $\sum_{n=0}^{\infty}|a_n|r^n<\infty$. On the whole [interval](../../../../../../../interval-mathematics.md) $[-r,r]$,

$$
|a_nx^n|\leq|a_n|r^n.
$$

The [Weierstrass M-test](../../../../../../../weierstrass-m-test.md) with $M_n=|a_n|r^n$ proves **[uniform convergence](../../../../../../../uniform-convergence.md) on $[-r,r]$.** It also gives the explicit tail estimate

$$
\boxed{\sup_{|x|\leq r}\left|\sum_{n=N+1}^{\infty}a_nx^n\right|\leq\sum_{n=N+1}^{\infty}|a_n|r^n\longrightarrow0.}
$$

For $r=0$ the [interval](../../../../../../../interval-mathematics.md) consists only of zero, and all positive-degree terms vanish. If $R=\infty$, the same argument applies to every finite $r$; if $R=0$, there is no $r\geq0$ with $r<R$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
