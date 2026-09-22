<h1 id="9/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [law of the unconscious statistician](../../../../../../law-of-the-unconscious-statistician.md) gives the improper integral

$$
\mathbb E(X^p)=\int_0^1x^p\,dx
=\lim_{\varepsilon\downarrow0}\frac{1-\varepsilon^{p+1}}{p+1}
=\boxed{\frac1{p+1}}\qquad(p>-1).
$$

In particular $\mathbb E(X)=1/2$ and $\mathbb E(X^2)=1/3$, so

$$
\boxed{\operatorname{Var}(X)=\frac13-\frac14=\frac1{12}.}
$$

For $p=-1$, $\int_\varepsilon^1x^{-1}dx=-\log\varepsilon\to+\infty$; for $p<-1$, the power integral also tends to $+\infty$. Thus **$\mathbb E(X^p)=+\infty$ for $p\leq-1$**, so there is no finite [expected value](../../../../../../expected-value-split.md). Negative powers need only be defined almost surely on $X>0$; the null event $X=0$ has no effect on this conclusion.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
