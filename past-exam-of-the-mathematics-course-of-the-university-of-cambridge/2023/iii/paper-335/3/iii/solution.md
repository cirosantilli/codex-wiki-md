<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the [Volterra integration operator](../../../../../../volterra-operator.md)

$$
(Af)(x)=\int_0^x f(t)\,dt,
$$

the [adjoint operator](../../../../../../adjoint-operator.md) is

$$
(A^*g)(x)=\int_x^1g(t)\,dt.
$$

Since $1/\sigma_n=(2n-1)\pi/2$, direct integration gives

$$
Au_n(x)
=\sqrt2\int_0^x\cos(t/\sigma_n)\,dt
=\sigma_n\sqrt2\sin(x/\sigma_n)
=\sigma_nv_n(x).
$$

Similarly,

$$
A^*v_n(x)
=\sqrt2\int_x^1\sin(t/\sigma_n)\,dt
=\sigma_n\sqrt2
\left(\cos(x/\sigma_n)-\cos(1/\sigma_n)\right)
=\sigma_nu_n(x),
$$

because $\cos((2n-1)\pi/2)=0$. The half-integer sine and cosine families are [orthonormal bases](../../../../../../orthonormal-basis.md) of $L^2([0,1])$, so $(\sigma_n,u_n,v_n)$ is a [singular system of a compact operator](../../../../../../singular-system-of-a-compact-operator.md).

The Tikhonov solution for noisy data $g^{(\delta)}$ is therefore

$$
\boxed{
f_\alpha(x)=
\sum_{n=1}^{\infty}
\frac{\sigma_n}{\sigma_n^2+\alpha}
\langle g^{(\delta)},v_n\rangle u_n(x)}.
$$

Writing out the [inner product](../../../../../../inner-product.md) and the singular functions makes this explicit:

$$
\boxed{
f_\alpha(x)=2\sum_{n=1}^{\infty}
\frac{\sigma_n}{\sigma_n^2+\alpha}
\cos\left(\frac{x}{\sigma_n}\right)
\int_0^1g^{(\delta)}(t)
\sin\left(\frac{t}{\sigma_n}\right)\,dt,
\qquad
\sigma_n=\frac{2}{(2n-1)\pi}.}
$$

The factors $\sigma_n/(\sigma_n^2+\alpha)$ suppress the unstable reciprocal growth $1/\sigma_n$ at high index.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
