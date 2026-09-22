<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Using $(Rf)'=\int_0^1f-f$ and [integration by parts](../../../../../integration-by-parts.md), with $\phi$ a [test function](../../../../../test-function.md), gives

$$
\int_0^1Rf\,\phi'=\int_0^1f\phi-\left(\int_0^1f\right)\left(\int_0^1\phi\right).
$$

For each $k\geq1$, apply the same identity to $R^kf$ and the [test function](../../../../../test-function.md) $\phi^{(k)}$. Since $\int_0^1\phi^{(k)}=0$, it gives

$$
\int_0^1R^{k+1}f\,\phi^{(k+1)}=\int_0^1R^kf\,\phi^{(k)}.
$$

Starting from $k=1$ and iterating proves

$$
\boxed{\int_0^1f\phi-\left(\int_0^1f\right)\left(\int_0^1\phi\right)
=\int_0^1R^kf\,\phi^{(k)}\quad(k\geq1).}
$$

The intermediate means disappear because derivatives of a [test function](../../../../../test-function.md) have zero integral; no assumption that $R^kf$ has zero mean is needed.

For the bound, write

$$
Rf(x)=\int_0^1\bigl(x-\mathbf1_{\{t<x\}}\bigr)f(t)\,dt.
$$

The [triangle inequality](../../../../../triangle-inequality.md) and [Fubini's theorem](../../../../../fubini-s-theorem.md) imply

$$
\begin{aligned}
\|Rf\|_{L^1}
&\leq\int_0^1|f(t)|\left[\int_0^t x\,dx+\int_t^1(1-x)\,dx\right]dt\\
&=\frac12\int_0^1\bigl[t^2+(1-t)^2\bigr]|f(t)|\,dt
\leq\frac12\|f\|_{L^1}.
\end{aligned}
$$

Thus $\boxed{c=\tfrac12\text{ is valid}}$, and every iterate $R^kf$ is in the [L1 space](../../../../../l1-space.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the distribution theory course of the University of Oxford](../../../../split.md)
6. [Distribution theory course of the University of Oxford](../../../../../distribution-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
