<h1 id="4/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The printed numerical example reverses the digits and contradicts both definitions.** With the stated last-digit definition, $[Z]=17$ gives $X=7$, $Y=1$. Use those definitions throughout.

Put $q=e^{-\lambda}\in(0,1)$ and $N=\lfloor Z\rfloor$. The [exponential distribution](../../../../../../../exponential-distribution.md) gives

$$
\mathbb P(N=n)=\mathbb P(n\le Z<n+1)=(1-q)q^n,\qquad n\ge0.
$$

The [Euclidean division](../../../../../../../euclidean-division.md) $N=10Y+X$ has unique remainder $X\in\{0,\ldots,9\}$ and quotient $Y\in\{0,1,\ldots\}$. Thus the [joint probability mass function](../../../../../../../joint-probability-mass-function.md) is

$$
\boxed{p_{X,Y}(x,y)=(1-q)q^{x+10y},\quad
x=0,\ldots,9,\ y=0,1,\ldots,}
$$

and zero otherwise. This is [decimal digit decomposition of a geometric random variable](../../../../../../../decimal-digit-decomposition-of-a-geometric-random-variable.md). Following the erroneous example instead would require different definitions and would not answer the stated question.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Mathematics III resit](../../../../mathematics-iii-resit-split.md)
5. [Prelims](../../../../split.md)
6. [Undated](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
