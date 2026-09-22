<h1 id="29a/solution">Solution</h1>

↑ **Parent:** [29A](../29a.md)

The [heat kernel](../../../../../heat-kernel.md) is $H_t(x)=(4\pi t)^{-1/2}e^{-x^2/(4t)}$, so the homogeneous solution for smooth bounded data is **$u(t,x)=(H_t*g)(x)$**. Differentiating under the integral gives the [heat equation](../../../../../heat-equation.md), and the approximate-identity property gives the initial value.

For a [tempered distribution](../../../../../tempered-distribution.md), its derivative is defined by $\langle T',\psi\rangle=-\langle T,\psi'\rangle$ for every Schwartz test function. A fundamental solution of a constant-coefficient operator $P$ is a distribution $E$ satisfying $PE=\delta_0$. Put $E(x)=e^{-|x|}/2$. Away from zero, $E''=E$; its first derivative has jump $-1$ at zero. Distributional differentiation therefore gives $E''=E-\delta_0$, and

$$
\boxed{(-D^2+1)E=\delta_0.}
$$

For an ansatz $u=e^tv$, the forced equation becomes $(1-D^2)v=\phi$. With Fourier convention $\widehat v(k)=\int e^{-ikx}v(x)dx$, its unique solution in the [Schwartz space](../../../../../schwartz-space.md) is

$$
\boxed{\widehat v(k)=\frac{\widehat\phi(k)}{1+k^2},\qquad v=E*\phi.}
$$

The smooth multiplier and its derivatives have [polynomial](../../../../../polynomial-split.md) bounds, so this quotient is Schwartz. For uniqueness, multiplication of the difference's [Fourier transform](../../../../../fourier-transform.md) by $1+k^2$ gives zero, forcing the difference to vanish.

Subtract this particular solution and evolve the remaining initial data by the [heat kernel](../../../../../heat-kernel.md):

$$
\boxed{u(t,x)=e^tv(x)+H_t*(f-v)(x).}
$$

For smooth bounded $f$, the second term remains uniformly bounded, so $e^{-t}u(t,\cdot)\to v$ uniformly. If additionally $f-v$ is integrable, its uniform [norm](../../../../../norm.md) is $O(t^{-1/2})$, so the remainder itself decays. General bounded data need not have a decaying heat remainder, and no such stronger claim follows without a condition on the data. The homogeneous uniqueness assertion is understood in the bounded or usual tempered-growth solution class; the uniqueness of the particular Schwartz ansatz is unconditional within that stated class.

## ↑ Ancestors (10)

1. [29A](../29a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
