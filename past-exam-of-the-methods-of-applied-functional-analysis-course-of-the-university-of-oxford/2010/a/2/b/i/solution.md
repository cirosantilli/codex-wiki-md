<h1 id="a/2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose a standard [mollifier](../../../../../../mollifier.md) $\rho\in C_0^\infty(\mathbb R^n)$ with $\rho\geq0$, $\int\rho=1$ and support in the unit ball, and set $\rho_\varepsilon(z)=\varepsilon^{-n}\rho(z/\varepsilon)$. Define the [convolution](../../../../../../convolution.md)

$$
\boxed{u_\varepsilon(x)=(\rho_\varepsilon*u)(x)=\int_{\mathbb R^n}\rho_\varepsilon(x-z)u(z)\,dz.}
$$

The smoothing properties of a [mollifier](../../../../../../mollifier.md) give $u_\varepsilon\in C^\infty$ and $\partial_ju_\varepsilon=\rho_\varepsilon*D_ju$. Apply the [chain rule](../../../../../../chain-rule.md) to $t\mapsto u_\varepsilon(y+t(x-y))$ and integrate its derivative by the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md):

$$
\boxed{u_\varepsilon(x)-u_\varepsilon(y)=\int_0^1\nabla u_\varepsilon(y+t(x-y))\cdot(x-y)\,dt.}
$$

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [A](../../../../a.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the methods of applied functional analysis course of the University of Oxford](../../../../../split.md)
7. [Methods of applied functional analysis course of the University of Oxford](../../../../../../methods-of-applied-functional-analysis-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
