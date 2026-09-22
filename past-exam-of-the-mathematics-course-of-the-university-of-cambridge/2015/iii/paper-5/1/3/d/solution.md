<h1 id="1/3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The tangent-line inequality for a differentiable [concave function](../../../../../../../concave-function.md) is $f(r)\le f(s)+f'(s)(r-s)$. Taking $r=u=U_x$ and using the [Hamilton-Jacobi equation](../../../../../../../hamilton-jacobi-equation.md) yields

$$
U_t+f'(s)U_x=f'(s)u-f(u)\ge sf'(s)-f(s).
$$

Along $x(\tau)=x_0+\tau f'(s)$, the [chain rule](../../../../../../../chain-rule.md) identifies the left side with $dU(\tau,x(\tau))/d\tau$. Integrating gives

$$
\boxed{U(t,x_0+t f'(s))-U(0,x_0)\ge t\bigl(sf'(s)-f(s)\bigr).}
$$

Strict [concavity](../../../../../../../concave-function.md) makes equality possible exactly when $u=s$ along the line, which will select the maximizing [characteristic curve](../../../../../../../characteristic-curve.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [1](../../../1.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
