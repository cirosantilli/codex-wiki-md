<h1 id="12b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $U(s,x)=\mathcal L_t\{u(t,x)\}$. The initial data turn the wave equation into

$$
-\frac{\partial^2U}{\partial x^2}+s^2U=f(x).
$$

Using the Green [function](../../../../../../function-split.md) from part (ii) with $m=s$ gives

$$
U(s,x)=\frac1{2s}\int_{-\infty}^{\infty}
 e^{-s|x-y|}f(y)\,dy.
$$

Since

$$
\mathcal L^{-1}\!\left\{\frac{e^{-as}}s\right\}=H(t-a),
$$

we obtain the [D'Alembert formula with initial velocity](../../../../../../d-alembert-formula-with-initial-velocity.md)

$$
\boxed{
u(t,x)=\frac12\int_{-\infty}^{\infty}
 H(t-|x-y|)f(y)\,dy
=\frac12\int_{x-t}^{x+t}f(y)\,dy}.
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [12B](../../12b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
