<h1 id="17b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The insulated boundary imposes the [Neumann boundary condition](../../../../../../neumann-boundary-condition.md) $T_{x_1}(0,x_2,t)=0$. Use the [method of images](../../../../../../method-of-images.md) by reflecting the initial data evenly across $x_1=0$. At the origin, the original sector and its reflection contribute equally. Using the given two-dimensional [heat kernel](../../../../../../heat-kernel.md),

$$
T(0,0,t)=\frac{2T_0}{4\pi Kt}\int_{-\pi/4}^{\pi/4}\int_1^2e^{-r^2/(4Kt)}r\,dr\,d\theta
=\frac{T_0}{2}\left(e^{-1/(4Kt)}-e^{-1/(Kt)}\right).
$$

Differentiation gives

$$
\frac{dT}{dt}=\frac{T_0}{8Kt^2}\left(e^{-1/(4Kt)}-4e^{-1/(Kt)}\right).
$$

This vanishes exactly when $e^{3/(4Kt)}=4$. Its sign is positive before that time and negative afterwards. Moreover $T\to0$ as $t\downarrow0$ and as $t\to\infty$. Therefore this is the unique global maximum:

$$
\boxed{t_{\max}=\frac3{8K\log2},\qquad T_{\max}=\frac{3T_0}{8\,4^{1/3}}}.
$$

The factor two from the insulated-boundary reflection is essential; applying the full-plane [heat kernel](../../../../../../heat-kernel.md) only to the unreflected sector would give half the temperature.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17B](../../17b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
