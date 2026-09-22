<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use unit speed and write the [Cauchy data](../../../../../../cauchy-data.md) as $u(0)=f$, $u_t(0)=g$. For finite-energy data define the [wave energy estimate](../../../../../../wave-energy-estimate.md) quantity

$$
E(t)=\frac12\int_{\mathbb R^n}\bigl(u_t^2+|\nabla_xu|^2\bigr)\,dx.
$$

Multiply $u_{tt}-\Delta_xu=0$ by $u_t$ and use [integration by parts](../../../../../../integration-by-parts.md). With compact support or sufficient decay the boundary flux is zero, so

$$
E'(t)=\int u_t(u_{tt}-\Delta_xu)\,dx=0,
\qquad
\boxed{\|u_t(t)\|_2^2+\|\nabla_xu(t)\|_2^2=\|g\|_2^2+\|\nabla f\|_2^2.}
$$

For general finite-energy solutions, cutoff or approximation arguments justify this identity; equivalently the local estimate below, applied in both time directions and with radii tending to infinity, gives the same equality. Arbitrary [smooth](../../../../../../smooth-function.md) data need not have finite global energy; then the global bound with an infinite right side is uninformative, while the local estimate remains useful.

If $f\in H^1$ and $g\in L^2$, the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) and the [wave energy estimate](../../../../../../wave-energy-estimate.md) further give

$$
\|u(t)\|_2\leq\|f\|_2+|t|\sqrt{\|g\|_2^2+\|\nabla f\|_2^2}.
$$

Together these yield an a priori bound for $\|u(t)\|_{H^1}+\|u_t(t)\|_2$ on each bounded time interval. No existence assumption is proved by the estimate itself; it controls any sufficiently regular solution.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
