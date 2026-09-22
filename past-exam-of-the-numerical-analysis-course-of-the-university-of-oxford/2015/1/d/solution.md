<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $E(h)$ for the supplied approximation. The [asymptotic expansion](../../../../asymptotic-expansion-split.md) is

$$
Y=E(h)+ch^2+r(h),\qquad r(h)=O(h^3),
$$

where $O$ is [Big O notation](../../../../big-o-notation.md). At the refined parameter $h/3$,

$$
Y=E(h/3)+\frac{ch^2}{9}+r(h/3).
$$

Multiply this identity by nine and subtract the first one. The unknown leading [truncation error](../../../../truncation-error.md) coefficient cancels:

$$
8Y=9E(h/3)-E(h)+9r(h/3)-r(h).
$$

Thus the [Richardson extrapolation](../../../../richardson-extrapolation.md) estimate is

$$
Y_{\rm ext}(h)=\frac{9E(h/3)-E(h)}8,\qquad
Y-Y_{\rm ext}(h)=O(h^3).
$$

The two supplied values give

$$
\boxed{Y_{\rm ext}(1)=\frac{9\cdot3-2}{8}=\frac{25}{8}=3.125.}
$$

The correction to the finer approximation is $(3-2)/8=1/8$. Neglecting the higher-order remainder would also give $c=9/8$.

The conclusion is asymptotic: the leading error order improves from two to at least three when both parameter values are in the range of the stated [asymptotic expansion](../../../../asymptotic-expansion-split.md). With no bound on the remainder constant, the two finite observations alone do not guarantee that $25/8$ is closer to $Y$. Indeed, for any proposed value $L$, the [polynomial](../../../../polynomial-split.md) model

$$
E(h)=L-c_Lh^2-d_Lh^3,\qquad
c_L=13L-\frac{79}{2},\qquad d_L=\frac{75}{2}-12L
$$

satisfies $E(1)=2$, $E(1/3)=3$ and the required [asymptotic expansion](../../../../asymptotic-expansion-split.md) with true [limit](../../../../limit-of-a-function.md) $L$. This is why [finite observations do not certify Richardson extrapolation accuracy](../../../../finite-observations-do-not-certify-richardson-extrapolation-accuracy.md): asymptotic cancellation provides an improved-order estimator, while a numerical error certificate needs quantitative remainder information.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
