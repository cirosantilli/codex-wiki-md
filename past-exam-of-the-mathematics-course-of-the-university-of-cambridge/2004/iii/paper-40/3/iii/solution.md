<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use [uniform-envelope rejection sampling for a beta distribution](../../../../../../uniform-envelope-rejection-sampling-for-a-beta-distribution.md). Put $r(x)=x^{a-1}(1-x)^{b-1}$ for $0<x<1$ and choose $M=\sup r$. For $a,b>1$, [differentiation](../../../../../../differentiation.md) of $\log r$ gives the mode $(a-1)/(a+b-2)$, so

$$
M=\left(\frac{a-1}{a+b-2}\right)^{a-1}
\left(\frac{b-1}{a+b-2}\right)^{b-1}.
$$

If $a=1$ or $b=1$, take $M=1$; this also covers $a=b=1$. Draw $X=U_{2j-1}$ and accept it if

$$
\boxed{U_{2j}\leq\frac{r(X)}M.}
$$

Otherwise continue with the next [independent](../../../../../../independent-random-variables.md) pair. The [probability](../../../../../../probability.md) of acceptance is $\int_0^1r(x)\,dx/M=B(a,b)/M>0$, so the procedure terminates almost surely. Conditional on acceptance, the [probability density function](../../../../../../probability-density-function.md) is proportional to $r(x)$, hence is exactly the [Beta distribution](../../../../../../beta-distribution.md) of parameters $a,b$. The restriction $a,b\geq1$ guarantees the bounded uniform envelope.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
