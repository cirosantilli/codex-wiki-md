<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Fokker-Planck equation](../../../../../../fokker-planck-equation.md) corresponds to the [Itô diffusion](../../../../../../ito-diffusion.md)

$$
\boxed{dX=v(X)dt+\sqrt{2D}\,dW,}
$$

absorbed at $0$ and reflected at $L$.

For $v(x)=x$, an Euler--Maruyama proposal is

$$
Y=X_n+X_n\Delta t+\sqrt{2D\Delta t}\,Z_n,
\qquad Z_n\sim N(0,1).
$$

If $Y\leq0$, kill the path. If $X_n>0$ and $Y>0$, an endpoint-only test can miss a crossing. Conditional on the endpoints, the local [Brownian bridge](../../../../../../brownian-bridge.md) crossing probability is

$$
\boxed{p_{\rm cross}=\exp\left(-\frac{X_nY}{D\Delta t}\right).}
$$

Kill the path with this probability; otherwise impose reflection at $L$ by replacing an overshoot $Y>L$ with $2L-Y$ and set $X_{n+1}=Y$. Repeated reflection handles very rare multiple overshoots, and the approximation converges as $\Delta t\to0$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
