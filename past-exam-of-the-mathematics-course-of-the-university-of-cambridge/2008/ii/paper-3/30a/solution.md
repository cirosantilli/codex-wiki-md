<h1 id="30a/solution">Solution</h1>

↑ **Parent:** [30A](../30a.md)

If $g'$ never vanishes on $[a,b]$, [integration by parts](../../../../../integration-by-parts.md) gives $I(\lambda)=[f(t)e^{i\lambda g(t)}/(i\lambda g'(t))]_a^b-(i\lambda)^{-1}\int_a^b(f/g')'e^{i\lambda g(t)}\,dt$, hence $\boxed{I(\lambda)=O(\lambda^{-1})}$ for smooth $f,g$. Endpoint terms usually attain this order; special cancellation can give faster decay.

For the final integral, take the imaginary part of $\int_0^1e^{i\lambda(t^3-t)}\,dt$. Its sole stationary point is $t_0=1/\sqrt3$, with $g(t_0)=-2/(3\sqrt3)$ and $g''(t_0)=2\sqrt3$. The [stationary phase](../../../../../stationary-phase-method.md) formula in part (a) therefore gives

$$
\boxed{J(\lambda)=\sqrt{\frac\pi{\lambda\sqrt3}}\sin\left(\frac\pi4-\frac{2\lambda}{3\sqrt3}\right)+O(\lambda^{-1}).}
$$

## ↑ Ancestors (10)

1. [30A](../30a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
