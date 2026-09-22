<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $h\ge0$ be proportional to the target [probability density function](../../../../../../probability-density-function.md), with $0<Z=\int h(x)\,dx<\infty$. Define the [ratio-of-uniforms method](../../../../../../ratio-of-uniforms-method.md) through the region

$$
A_h=\{(u,v):u>0,\ u^2\le h(v/u)\}.
$$

Draw $(U,V)$ uniformly with respect to area on $A_h$ and return $X=V/U$. To prove its law, change variables from $(u,x)$ to $(u,v)=(u,ux)$. The [Jacobian determinant](../../../../../../jacobian-determinant.md) is $u$, and the allowed interval for $u$ is $0<u\le\sqrt{h(x)}$. Consequently

$$
\operatorname{area}(A_h)=\int_{\mathbb R}\int_0^{\sqrt{h(x)}}u\,du\,dx=\frac Z2.
$$

The joint density of $(U,X)$ is therefore $2u/Z$ on that interval. Integrating out $u$ gives

$$
\boxed{f_X(x)=\int_0^{\sqrt{h(x)}}\frac{2u}{Z}\,du=\frac{h(x)}Z.}
$$

For an already normalized density, $Z=1$ and the region has area $1/2$. The name refers to the two coordinates of a uniformly sampled region; drawing two unrelated uniforms on arbitrary intervals and taking their ratio would not give the target law.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
