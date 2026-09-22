<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

In [polar coordinates](../../../../../polar-coordinates.md), the [Laplace equation](../../../../../laplace-equation.md) is

$$
\phi_{rr}+r^{-1}\phi_r+r^{-2}\phi_{\theta\theta}=0.
$$

For a single-valued, $2\pi$-periodic [harmonic function](../../../../../harmonic-function.md) on an annulus, [separation of variables](../../../../../separation-of-variables.md) and its angular [Fourier series](../../../../../fourier-series-split.md) give

$$
\phi=a_0+b_0\log r+\sum_{n\geq1}\left[(a_nr^n+b_nr^{-n})\cos n\theta+(c_nr^n+d_nr^{-n})\sin n\theta\right].
$$

Indeed a nonzero angular mode has radial equation $r^2R''+rR'-n^2R=0$, with solutions $r^{\pm n}$; the zero mode has solutions 1 and $\log r$. This expression describes the periodic annular problem here; angular terms not periodic, such as $\theta$, are excluded.

Decay at the origin leaves only positive powers in the interior, and decay at infinity leaves only negative powers in the exterior. Continuity on the unit circle matches the corresponding [Fourier coefficients](../../../../../fourier-coefficient.md). If the common cosine coefficient is $K_n$, the interior and exterior terms are $K_nr^n\cos n\theta$ and $K_nr^{-n}\cos n\theta$. Their exterior-minus-interior radial [derivative](../../../../../derivative.md) at the circle is $-2nK_n\cos n\theta$. Thus [harmonic matching across a circle with a derivative jump](../../../../../harmonic-matching-across-a-circle-with-a-derivative-jump.md) gives $K_2=-1/4$, $K_4=-1/8$, and zero for every other sine or cosine mode. Consequently

$$
\boxed{\phi(r,\theta)=
\begin{cases}
-\frac14r^2\cos2\theta-\frac18r^4\cos4\theta,&0<r<1,\\
-\frac14r^{-2}\cos2\theta-\frac18r^{-4}\cos4\theta,&r>1.
\end{cases}}
$$

Each branch satisfies the [Laplace equation](../../../../../laplace-equation.md) and its respective decay condition. Both give $-\cos2\theta/4-\cos4\theta/8$ at $r=1$, and direct differentiation gives the required jump $\cos2\theta+\cos4\theta$. The same mode calculation leaves no nonzero homogeneous solution in this class.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
