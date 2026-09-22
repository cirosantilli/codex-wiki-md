<h1 id="15f/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Part (i) gives $\mathcal L(t)=1/s^2$ and $\mathcal L(te^{-t})=1/(s+1)^2$. The [convolution theorem for Laplace transforms](../../../../../../convolution-theorem-for-laplace-transforms.md) therefore gives

$$
f(t)=\int_0^t(t-v)ve^{-v}\,dv=t\int_0^tve^{-v}\,dv-\int_0^tv^2e^{-v}\,dv.
$$

Repeated [integration by parts](../../../../../../integration-by-parts.md) yields

$$
\int_0^tve^{-v}\,dv=1-(t+1)e^{-t},\qquad\int_0^tv^2e^{-v}\,dv=2-(t^2+2t+2)e^{-t}.
$$

Substitution gives **$f(t)=t-2+(t+2)e^{-t}$**, agreeing with the [contour integration](../../../../../../contour-integration.md) result.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [15F](../../15f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
