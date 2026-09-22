<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $H=\sup_{\overline B_1}\lVert D^2g\rVert$. For $x,x_0\in\partial B_1$, the [Taylor theorem with Lagrange remainder](../../../../../../taylor-theorem-with-lagrange-remainder.md) and $|x-x_0|^2=2x_0\mathbin\cdot(x_0-x)$ give

$$
|g(x)-g(x_0)-Dg(x_0)\mathbin\cdot(x-x_0)|
\leq Hx_0\mathbin\cdot(x_0-x).
$$

Therefore

$$
b_{x_0}^{\pm}(x)=g(x_0)+Dg(x_0)\mathbin\cdot(x-x_0)
\pm Hx_0\mathbin\cdot(x_0-x)
$$

are affine upper and lower barriers, agree with $g$ at $x_0$, and have Lipschitz constant at most $K=\sup_{\overline B_1}|Dg|+H$. Thus $g$ has the [bounded slope condition](../../../../../../bounded-slope-condition.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
