# Laplace integral solution of a singular third-order equation

↑ **Parent:** [Laplace integral method for a differential equation](laplace-integral-method-for-a-differential-equation.md)

For $x>0$, substituting $y(x)=\int_\gamma e^{xt}f(t)\,dt$ into $xy^{(3)}+2y=0$ and integrating by parts gives

$$
[e^{xt}t^3f(t)]_{\partial\gamma}
+\int_\gamma e^{xt}\{2f-(t^3f)'\}\,dt=0.
$$

The amplitude equation $(t^3f)'=2f$ has solution $f(t)=Ct^{-3}e^{-1/t^2}$. On $\gamma=(-\infty,0)$ both endpoint terms vanish, and hence

$$
y(x)=C\int_{-\infty}^0e^{xt-t^{-2}}t^{-3}\,dt
=C_1\int_0^\infty u e^{-u^2-x/u}\,du.
$$

## ↑ Ancestors (7)

1. [Laplace integral method for a differential equation](laplace-integral-method-for-a-differential-equation.md)
2. [Modified Bessel function](modified-bessel-function.md)
3. [Bessel function](bessel-function.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2/7d/b/solution.md)
