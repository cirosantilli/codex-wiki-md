<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

Put $u=\varepsilon v+O(\varepsilon^2)$. The [linearization](../../../../../linearization.md) at the zero solution is

$$
v_t=Dv_{xx}+f'(0)v,\qquad v(0,t)=v(L,t)=0.
$$

The appropriate [Fourier sine series](../../../../../fourier-sine-series.md) is

$$
v(x,t)=\sum_{n\ge1}a_n(t)\sin(n\pi x/L),\qquad
a_n(0)=\frac2L\int_0^Lu_0(x)\sin(n\pi x/L)\,dx.
$$

[Orthogonality](../../../../../orthogonal-vectors.md) of the modes gives

$$
a_n'(t)=\left(f'(0)-D(n\pi/L)^2\right)a_n(t).
$$

Thus each mode grows or decays exponentially with its own [eigenvalue](../../../../../eigenvalue.md), and the largest growth rate is the $n=1$ value. Strict [linear stability analysis](../../../../../linear-stability.md), meaning decay of every mode, is equivalent to

$$
\boxed{L<\pi\sqrt{\frac D{f'(0)}}.}
$$

At equality the first mode is neutral in the [linearization](../../../../../linearization.md); the nonlinear terms decide its subsequent behavior. Above this length the first mode grows, giving linear instability.

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
