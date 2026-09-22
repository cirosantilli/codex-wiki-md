<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

The [Laplace integral method for a differential equation](../../../../../laplace-integral-method-for-a-differential-equation.md) seeks

$$
y(z)=\int_Ce^{zt}f(t)\,dt.
$$

Differentiating under the integral and substituting into

$$
zy''+y'-zy=0
$$

gives

$$
\int_Ce^{zt}\left[z(t^2-1)f(t)+tf(t)\right]dt=0.
$$

Since $ze^{zt}=\partial_te^{zt}$, integration by parts yields

$$
\left[e^{zt}(t^2-1)f(t)\right]_{\partial C}
-\int_Ce^{zt}\left[(t^2-1)f'(t)+tf(t)\right]dt=0.
$$

It is therefore enough to choose $f$ and $C$ so that

$$
(t^2-1)f'(t)+tf(t)=0
$$

and the boundary term vanishes. Solving the first-order equation on $-1<t<1$ gives

$$
f(t)=\frac{K}{\sqrt{1-t^2}}.
$$

Take $C$ to be the interval $[-1,1]$. Although $f$ has integrable endpoint singularities,

$$
(t^2-1)f(t)=-K\sqrt{1-t^2}
$$

vanishes at both endpoints, so the boundary term is zero. Thus

$$
y(z)=K\int_{-1}^1\frac{e^{zt}}{\sqrt{1-t^2}}\,dt.
$$

At $z=0$, substituting $t=\sin\theta$ gives

$$
\int_{-1}^1\frac{dt}{\sqrt{1-t^2}}=\pi.
$$

The normalization $y(0)=1$ therefore sets $K=1/\pi$. By the defining regularity and normalization of the [modified Bessel function](../../../../../modified-bessel-function.md), this proves the [real integral representation of the modified Bessel function I0](../../../../../real-integral-representation-of-the-modified-bessel-function-i0.md):

$$
\boxed{I_0(z)=\frac1\pi\int_{-1}^1
\frac{e^{zs}}{\sqrt{1-s^2}}\,ds}.
$$

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
