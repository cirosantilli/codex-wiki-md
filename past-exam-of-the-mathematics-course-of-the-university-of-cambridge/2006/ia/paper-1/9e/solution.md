<h1 id="9e/solution">Solution</h1>

↑ **Parent:** [9E](../9e.md)

The [intermediate value theorem](../../../../../intermediate-value-theorem.md) states that a continuous real-valued function on $[a,b]$ takes every value between $f(a)$ and $f(b)$. To prove it, suppose $f(a)<k<f(b)$ and repeatedly bisect the interval, keeping endpoints whose function values bracket $k$. The resulting nested closed intervals have lengths tending to zero and a common point $c$ by [completeness of the real numbers](../../../../../completeness-of-the-real-numbers.md). Both endpoint sequences tend to $c$, so [continuity](../../../../../continuous-function.md) implies $f(c)=k$. Endpoint values are immediate, and reversing the inequalities handles $f(a)>f(b)$.

For the derivative assertion, put $m=(f(b)-f(a))/(b-a)$. The [intermediate secant slope from endpoint derivatives](../../../../../intermediate-secant-slope-from-endpoint-derivatives.md) can be constructed in three cases. If $m=k$, take $[a',b']=[a,b]$. If $m>k$, the function

$$
g(x)=\frac{f(x)-f(a)}{x-a},\qquad g(a)=f'(a),
$$

is continuous on $[a,b]$: differentiability at $a$ supplies the endpoint limit, and differentiability elsewhere implies continuity. Since $g(a)<k<g(b)$, the [intermediate value theorem](../../../../../intermediate-value-theorem.md) gives $x\in(a,b)$ with $g(x)=k$. Take $[a',b']=[a,x]$.

If $m<k$, use instead

$$
h(x)=\frac{f(b)-f(x)}{b-x},\qquad h(b)=f'(b).
$$

Its continuous endpoint extension satisfies $h(a)<k<h(b)$, so there is $y\in(a,b)$ with $h(y)=k$. Take $[a',b']=[y,b]$. In every case,

$$
\frac{f(b')-f(a')}{b'-a'}=k.
$$

The [mean value theorem](../../../../../mean-value-theorem.md) on this subinterval now gives

$$
\boxed{\text{some }c\in(a,b)\text{ satisfies }f'(c)=k.}
$$

This proves the [Darboux theorem for derivatives](../../../../../darboux-s-theorem-analysis.md) without assuming that $f'$ is continuous.

## ↑ Ancestors (10)

1. [9E](../9e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
