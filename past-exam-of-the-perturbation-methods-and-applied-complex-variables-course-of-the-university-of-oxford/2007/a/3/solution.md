<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For fixed nonzero $x$, expand the denominator geometrically:

$$
f(x)=\frac{e^{-x}}{x^2}-\epsilon^2\frac{e^{-x}}{x^4}+O(\epsilon^4).
$$

The effective expansion parameter is $\epsilon^2/x^2$, so the expansion fails when $x=O(\epsilon)$. In the [inner variable](../../../../inner-variable.md) $X=x/\epsilon$,

$$
F(X)=\frac{e^{-\epsilon X}}{\epsilon^2(1+X^2)}
=\frac{\epsilon^{-2}}{1+X^2}-\frac{\epsilon^{-1}X}{1+X^2}+O(1)
$$

for fixed $X$. Expanding the leading outer term toward $x=0$ gives $x^{-2}$ at leading order; expanding the leading inner term for large $X$ and returning to $x$ gives $\epsilon^{-2}X^{-2}=x^{-2}$. Thus the two one-term re-expansions match in $\epsilon\ll x\ll1$. The next common contribution is $-x^{-1}$ when the corresponding next inner order is retained.

On $x\geq\delta$, the relative denominator error is bounded by $\epsilon^2/\delta^2$, hence

$$
I_2=\left[1+O\left(\frac{\epsilon^2}{\delta^2}\right)\right]
\int_\delta^\infty\frac{e^{-x}}{x^2}dx.
$$

[Integration by parts](../../../../integration-by-parts.md) yields

$$
\int_\delta^\infty\frac{e^{-x}}{x^2}dx
=\frac{e^{-\delta}}{\delta}-\int_\delta^\infty\frac{e^{-x}}x\,dx
=\frac1\delta+\log\delta+O(1).
$$

For the last step split the remaining [integral](../../../../integral-split.md) at one: $\int_\delta^1 dx/x=-\log\delta$, and replacing $e^{-x}$ by one on that interval has a bounded error.

In the inner interval, $|e^{-x}-1|\leq x$ gives an explicit error estimate:

$$
I_1=\frac1\epsilon\arctan\frac\delta\epsilon
+O\left(\log\left(1+\frac{\delta^2}{\epsilon^2}\right)\right)
=\frac{\pi}{2\epsilon}-\frac1\delta
+O\left(\frac{\epsilon^2}{\delta^3}+
\log\left(1+\frac{\delta^2}{\epsilon^2}\right)\right).
$$

The $1/\delta$ terms cancel between regions. Every displayed remainder is $o(\epsilon^{-1})$ whenever $\epsilon/\delta\to0$ and $\delta\to0$; for example $\epsilon(\epsilon^2/\delta^3)=(\epsilon/\delta)^3$. Therefore the leading answer is independent of the arbitrary intermediate cutoff:

$$
\boxed{I\sim\frac{\pi}{2\epsilon}.}
$$

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../split.md)
5. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
