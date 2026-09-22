<h1 id="14b/solution">Solution</h1>

↑ **Parent:** [14B](../14b.md)

Since $x=r\cos\theta$, the function on the left of the defining expansion is $e^{ix}$. Therefore

$$
(\nabla^2+1)e^{ir\cos\theta}
=(\partial_x^2+\partial_y^2+1)e^{ix}=0,
$$

which is the two-dimensional [Helmholtz equation](../../../../../helmholtz-equation.md).

In polar coordinates,

$$
\nabla^2=\frac{\partial^2}{\partial r^2}
+\frac1r\frac\partial{\partial r}
+\frac1{r^2}\frac{\partial^2}{\partial\theta^2}.
$$

Substitute the defining [Fourier cosine series](../../../../../fourier-cosine-series.md) and equate the coefficient of each $\cos(n\theta)$. Its angular second derivative contributes $-n^2$, so every [Bessel function](../../../../../bessel-function.md) $J_n$ satisfies

$$
J_n''+\frac1rJ_n'+\left(1-\frac{n^2}{r^2}\right)J_n=0,
$$

or equivalently the [Bessel differential equation](../../../../../bessel-differential-equation.md)

$$
\boxed{r^2J_n''+rJ_n'+(r^2-n^2)J_n=0}.
$$

Expand the exponential through cubic order and use

$$
\cos^2\theta=\frac{1+\cos2\theta}{2},
\qquad
\cos^3\theta=\frac{3\cos\theta+\cos3\theta}{4}.
$$

This gives

$$
e^{ir\cos\theta}
=1-\frac{r^2}{4}
+i\left(r-\frac{r^3}{8}\right)\cos\theta
-\frac{r^2}{4}\cos2\theta
-\frac{ir^3}{24}\cos3\theta+O(r^4).
$$

Comparing with $J_0+2\sum_{n\geq1}i^nJ_n\cos(n\theta)$ yields

$$
\boxed{J_0(r)=1-\frac{r^2}{4}+O(r^4)},
$$



$$
\boxed{J_1(r)=\frac r2-\frac{r^3}{16}+O(r^5),
\quad J_2(r)=\frac{r^2}{8}+O(r^4),
\quad J_3(r)=\frac{r^3}{48}+O(r^5)}.
$$

## ↑ Ancestors (10)

1. [14B](../14b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
