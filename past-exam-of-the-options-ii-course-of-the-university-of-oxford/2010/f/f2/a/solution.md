<h1 id="f/f2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Differentiability](../../../../../differentiability.md) at $x_0$ means that a [linear map](../../../../../linear-map.md) $A:\mathbb R^n\to\mathbb R^m$ exists with

$$
f(x_0+h)=f(x_0)+Ah+o(\|h\|).
$$

The map $A=Df(x_0)$ is the [total derivative](../../../../../total-derivative.md). A [linear map](../../../../../linear-map.md) between these finite-dimensional spaces is bounded, so $\|f(x_0+h)-f(x_0)\|\leq\|A\|\|h\|+o(\|h\|)\to0$. Thus [differentiability](../../../../../differentiability.md) implies [continuity](../../../../../continuous-function.md).

For the displayed two-variable function,

$$
0\leq\frac{x^4}{\sqrt{x^4+y^2}}\leq x^2\leq x^2+y^2.
$$

Writing $r=\sqrt{x^2+y^2}$ gives $|f(x,y)|/r\leq r\to0$. Therefore **it is differentiable at the origin, with derivative zero**.

Finally, put $h=x-x_0$, write $f(x_0+h)=Ah+r(h)$ with $r(h)=o(\|h\|)$, and $g(x_0+h)=g(x_0)+s(h)$ with $s(h)=o(1)$. Since $f(x_0)=0$,

$$
F(x_0+h)=\langle Ah,g(x_0)\rangle
+\langle Ah,s(h)\rangle+\langle r(h),g(x_0)+s(h)\rangle.
$$

By the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) the last two terms are $o(\|h\|)$: $A$ is bounded and $g(x_0)+s(h)$ stays bounded. Hence

$$
\boxed{DF(x_0)h=\langle Df(x_0)h,g(x_0)\rangle.}
$$

Only [continuity](../../../../../continuous-function.md) of $g$ at $x_0$ is needed, because the vanishing of $f(x_0)$ removes the term which would otherwise require differentiating $g$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [F2](../../f2.md)
3. [F](../../../f.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
