<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $x_0>a$, define

$$
l=\sup\{f(t):a\leq t<x_0\}.
$$

This nonempty [set](../../../../../../set-split.md) is bounded above by $f(x_0)$, so $l\leq f(x_0)$. Given $\varepsilon>0$, the [supremum](../../../../../../supremum.md) property supplies $s<x_0$ with $l-\varepsilon<f(s)\leq l$. Whenever $s<t<x_0$, [monotonicity](../../../../../../monotonic-function.md) gives

$$
l-\varepsilon<f(s)\leq f(t)\leq l.
$$

This proves the left-hand [one-sided limit](../../../../../../one-sided-limit.md) $f^-(x_0)=l$.

For $x_0<b$, define

$$
r=\inf\{f(t):x_0<t\leq b\}.
$$

Here $r\geq f(x_0)$. Choose $u>x_0$ with $r\leq f(u)<r+\varepsilon$, using the [infimum](../../../../../../infimum.md) property. For $x_0<t<u$, [monotonicity](../../../../../../monotonic-function.md) gives $r\leq f(t)\leq f(u)<r+\varepsilon$, proving the right-hand [one-sided limit](../../../../../../one-sided-limit.md) $f^+(x_0)=r$. Thus

$$
\boxed{f^-(x_0)\leq f(x_0)\leq f^+(x_0)}
$$

where the relevant [one-sided limits](../../../../../../one-sided-limit.md) exist, including the indicated single [one-sided limit](../../../../../../one-sided-limit.md) at each endpoint.

At an interior point, [continuity](../../../../../../continuous-function.md) implies both [one-sided limits](../../../../../../one-sided-limit.md) equal $f(x_0)$. Conversely, equality $f^-(x_0)=f^+(x_0)$ and the displayed inequalities force both to equal $f(x_0)$, giving [continuity](../../../../../../continuous-function.md). Therefore

$$
\boxed{f\text{ continuous at }x_0\in(a,b)\iff f^-(x_0)=f^+(x_0).}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
