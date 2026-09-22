<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $r=1-p$. Since

$$
\frac{d}{dx}\log(1-r e^{-\beta x})
=\frac{\beta r e^{-\beta x}}{1-r e^{-\beta x}},
$$

integration from zero to $x>0$ gives $F(x)=(C/\beta)[\log(1-r e^{-\beta x})-\log p]$. Letting $x\to\infty$ and imposing unit total [probability](../../../../../probability.md) gives

$$
\boxed{C=-\frac{\beta}{\log p}>0,\qquad
F(x)=\begin{cases}
0,&x\leq0,\\
1-\dfrac{\log(1-(1-p)e^{-\beta x})}{\log p},&x>0.
\end{cases}}
$$

The [probability density function](../../../../../probability-density-function.md) is positive for $x>0$ because $0<(1-p)e^{-\beta x}<1$. Consequently the [cumulative distribution function](../../../../../cumulative-distribution-function.md) is increasing, starts at zero and tends to one. This verifies that the derived [normalizing constant](../../../../../normalizing-constant.md) defines a [probability distribution](../../../../../probability-distribution-split.md). The family is the [exponential-logarithmic distribution](../../../../../exponential-logarithmic-distribution.md) with the complementary mixing parameter $r=1-p$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
