# Complementary error function tail bound

↑ **Parent:** [Complementary error function](complementary-error-function.md)

For every real $x>0$,

$$
\frac{e^{-x^2}}{\sqrt\pi(x+1/(2x))}<\operatorname{erfc}(x)<\frac{e^{-x^2}}{\sqrt\pi x}.
$$

For a short proof, put $I(x)=\int_x^\infty e^{-t^2}\,dt$. [Integration by parts](integration-by-parts.md) gives

$$
I(x)=\frac{e^{-x^2}}{2x}-\frac12\int_x^\infty\frac{e^{-t^2}}{t^2}\,dt.
$$

The last [integral](integral-split.md) is positive and strictly smaller than $I(x)/x^2$. Using these two inequalities gives the upper and lower bounds after multiplication by $2/\sqrt\pi$. Dividing both bounds by $e^{-x^2}/(\sqrt\pi x)$ also proves the leading [asymptotic equivalence](asymptotic-equivalence.md) by the [squeeze theorem](squeeze-theorem.md). For small positive $x$, the bounds remain true but can be loose; they are especially useful when the [Gaussian integral](gaussian-integral.md) tail is already small.

## ↑ Ancestors (10)

1. [Complementary error function](complementary-error-function.md)
2. [Error function](error-function.md)
3. [Gaussian integral](gaussian-integral.md)
4. [Integral](integral-split.md)
5. [Calculus](calculus-split.md)
6. [Real analysis](real-analysis-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Complementary error function](complementary-error-function.md)
