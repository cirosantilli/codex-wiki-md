<h1 id="s/s2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**The assertion is false for the algorithm as printed.** Its second output depends only on $V$. For $0<V\leq1/2$ its sine factor is nonnegative. For $1/2<V<1$, its radius is at most $\sqrt{2\log2}$, so in every case $Y\geq-\sqrt{2\log2}$. Therefore $\Pr(Y<-2)=0$, whereas a standard normal variable has positive [probability](../../../../../probability.md) below $-2$. The printed output cannot be a pair of independent standard normals.

The minimal correction is to use $U$ in both logarithms. Let $R=\sqrt{-2\log U}$, $\Theta=2\pi V$, and set $X=R\cos\Theta$, $Y=R\sin\Theta$. Independence of $U,V$ gives independent $R,\Theta$ with densities $re^{-r^2/2}$ for $r>0$ and $1/(2\pi)$ for the angle. The polar-coordinate Jacobian is $r$, so the joint Cartesian density is

$$
\boxed{f_{X,Y}(x,y)=\frac1{2\pi}e^{-(x^2+y^2)/2}
=\frac{e^{-x^2/2}}{\sqrt{2\pi}}\frac{e^{-y^2/2}}{\sqrt{2\pi}}.}
$$

This proves independent standard normal outputs for the corrected [Box-Muller transform](../../../../../box-muller-transform.md). The private transcription retains the source's original $\log V$ and records this correction separately.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [S2](../../s2.md)
3. [S](../../../s.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
