<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Divide the recurrence by $2k$ and substitute a smooth exact solution. Centered [Taylor expansions](../../../../../../taylor-expansion.md) in time and space give

$$
\frac{u(t+k)-u(t-k)}{2k}-\frac{u(x+\delta,y)-u(x-\delta,y)+u(x,y+\delta)-u(x,y-\delta)}{2\delta}
=\frac{k^2}{6}u_{ttt}-\frac{\delta^2}{6}(u_{xxx}+u_{yyy})+O(k^4+\delta^4).
$$

Thus the [leapfrog advection scheme](../../../../../../leapfrog-advection-scheme.md) is consistent with normalized residual $O(k^2+\delta^2)$. Its unnormalized defect is $O(k^3+k\delta^2)$. For a fixed $0<\nu<1/2$, the uniform two-level bound proved above and accumulation over $O(1/k)$ steps yield, for a sufficiently smooth solution,

$$
\max_{nk\leq T}\|e^n\|_{2,\delta}\leq C_{T,\nu}\bigl(\|e^0\|_{2,\delta}+\|e^1\|_{2,\delta}+k^2+\delta^2\bigr).
$$

Both starting levels must be supplied consistently; errors of order $k^2+\delta^2$ give second-order convergence. For general [square-integrable functions](../../../../../../square-integrable-function.md) as initial data, point sampling is not defined on equivalence classes. Use cell averages or another bounded grid projection, together with a bounded consistent startup. Approximate the initial data by smooth functions, apply the smooth-data convergence estimate, and use the uniform numerical and exact translation bounds to pass to the [L2 space](../../../../../../l2-space-is-a-hilbert-space.md) limit. This is the content of [Lax equivalence theorem](../../../../../../lax-equivalence-theorem.md) in the present setting.

At $\nu>1/2$ the growing [Fourier mode](../../../../../../fourier-mode.md) prevents general convergence. At the endpoint, initial data supported in increasingly narrow neighborhoods of the double root can have a second-level error of norm $O(k)$ but a final error of order one after $O(1/k)$ steps. These are vanishing starting errors, so the endpoint fails general two-level convergence as well. Consequently

$$
\boxed{0<\Delta t/\Delta x<1/2}
$$

is also the general convergence range, with a consistent stable initialization. Claims for a particular specially chosen endpoint startup would be a different, restricted assertion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
