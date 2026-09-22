<h1 id="30a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [Cauchy problem for a partial differential equation](../../../../../../cauchy-problem.md), suppose $a,b,c$ are $C^1$ near the lifted initial data, $\Gamma$ has a regular $C^1$ parametrization $(\xi(s),\eta(s))$, and the initial function $u_0(s)$ is $C^1$. The local existence and uniqueness theorem requires the [Noncharacteristic Cauchy data](../../../../../../noncharacteristic-cauchy-data.md) condition

$$
\boxed{a(\xi,\eta,u_0)\eta'(s)-b(\xi,\eta,u_0)\xi'(s)\ne0}
$$

at the starting point. Then there is a neighbourhood of that point carrying a unique $C^1$ classical solution attaining the initial values.

The [method of characteristics](../../../../../../method-of-characteristics.md) proves this by solving

$$
\frac{dx_1}{d\tau}=a(x_1,x_2,U),\quad\frac{dx_2}{d\tau}=b(x_1,x_2,U),\quad\frac{dU}{d\tau}=c(x_1,x_2,U),
$$

with initial values $(\xi(s),\eta(s),u_0(s))$ at $\tau=0$. Local existence for these ordinary differential equations gives a $C^1$ map. The noncharacteristic determinant is, up to sign, the Jacobian determinant of $(s,\tau)\mapsto(x_1,x_2)$ initially. The [inverse function theorem](../../../../../../inverse-function-theorem.md) makes this map locally invertible, defining $u(x_1,x_2)=U(s,\tau)$ and proving uniqueness along characteristics.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30A](../../30a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
