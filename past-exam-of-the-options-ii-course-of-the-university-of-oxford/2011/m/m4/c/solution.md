<h1 id="m/m4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At a fixed index, [independence](../../../../../independent-random-variables.md) and uniformity give

$$
p=P(X_s=Y_s)=\sum_{j=0}^{k-1}\frac1{k^2}=\frac1k.
$$

The match indicators are independent [Bernoulli trials](../../../../../bernoulli-trial.md). Thus the waiting times between successive matches are independent [geometric](../../../../../geometric-distribution.md) variables on $\{1,2,\ldots\}$ with success [probability](../../../../../probability.md) $p$. Their [moment-generating function](../../../../../moment-generating-function.md) is

$$
\sum_{r=1}^\infty p(1-p)^{r-1}e^{tr}
=\frac{pe^t}{1-(1-p)e^t},
$$

provided $(1-p)e^t<1$. Since $S_m$ is the sum of $m$ such waiting times,

$$
\boxed{M_{S_m}(t)=\left(\frac{e^t}{k-(k-1)e^t}\right)^m,
\qquad\mathbb ES_m=mk.}
$$

For $k>1$, the finite domain is $t<\log(k/(k-1))$. For $k=1$, every index is a match, so $S_m=m$ deterministically and the [moment-generating function](../../../../../moment-generating-function.md) is $e^{mt}$ for every real $t$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [M4](../../m4.md)
3. [M](../../../m.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
