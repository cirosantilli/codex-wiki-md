<h1 id="differential-equations/9/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The same [integration by parts](../../../../../integration-by-parts.md) with $p$ replaced by $p+c$ gives

$$
\boxed{\overline{te^{-ct}}(p)=\frac1{(p+c)^2}\qquad(\operatorname{Re}(p+c)>0).}
$$

For the remaining unnumbered requests, the [derivative](../../../../../derivative.md) and [convolution](../../../../../convolution.md) formulas, under the usual convergence hypotheses, are

$$
\overline{f'}(p)=p\bar f(p)-f(0),\qquad\overline{f*g}(p)=\bar f(p)\bar g(p),\qquad(f*g)(t)=\int_0^tf(t-s)g(s)\,ds.
$$

Applying them to the general equation yields $p\bar x-a+\bar k\bar x=\bar y$ and therefore

$$
\boxed{\bar x(p)=\frac{\bar y(p)+a}{p+\bar k(p)}.}
$$

For the particular data, $\bar y=1/p$, $\bar k=1/(p+2)$ and $a=0$, so

$$
\bar x(p)=\frac{p+2}{p(p+1)^2}=\frac2p-\frac2{p+1}-\frac1{(p+1)^2}.
$$

The four transforms above give

$$
\boxed{x(t)=2-(2+t)e^{-t},\qquad\lim_{t\to\infty}x(t)=2.}
$$

As a direct check, $x(0)=0$, $x'=(1+t)e^{-t}$, and

$$
\int_0^te^{-2(t-s)}x(s)\,ds=1-(1+t)e^{-t}.
$$

Adding the last two expressions gives one, verifying the original equation as well as the required limit.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [9](../../9.md)
3. [Differential equations](../../../differential-equations.md)
4. [2006](../../../../2006-split.md)
5. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
