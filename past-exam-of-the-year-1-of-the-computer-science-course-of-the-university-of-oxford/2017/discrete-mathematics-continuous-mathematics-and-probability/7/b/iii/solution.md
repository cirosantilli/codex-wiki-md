<h1 id="7/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $Y\sim\operatorname{Geom}(p)$, its mean is $1/p$, so the [size-biased probability generating function](../../../../../../size-biased-probability-generating-function.md) is

$$
G_{\widetilde Y}(s)=\frac{p^2s}{(1-(1-p)s)^2}.
$$

Choose **$X_1,X_2$ independent with distribution $\operatorname{Geom}(p)$**. Their shifted sum has generating function, initially for $s>0$,

$$
G_{X_1+X_2-1}(s)=\frac1s\left(\frac{ps}{1-(1-p)s}\right)^2=G_{\widetilde Y}(s),
$$

with both sides continuous and zero at $s=0$. Equality of [probability generating functions](../../../../../../probability-generating-function.md) proves

$$
\boxed{\widetilde Y\overset d=X_1+X_2-1.}
$$

Equivalently, $X_1+X_2=k+1$ has $k$ possible positive summand pairs, each of probability $p^2(1-p)^{k-1}$, matching the [size-biased geometric distribution](../../../../../../size-biased-geometric-distribution.md) probabilities.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
