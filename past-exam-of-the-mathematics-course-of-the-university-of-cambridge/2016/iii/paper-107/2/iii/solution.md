<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Fix $x_0\in\partial\Omega$, $\varepsilon>0$, and the [power barrier for an exterior cone](../../../../../../power-barrier-for-an-exterior-cone.md) $g$ from part (i). Write $M=\|f\|_\infty$. By [continuity](../../../../../../continuous-function.md) of the boundary data, there is $\rho>0$ such that $|\varphi(x)-\varphi(x_0)|<\varepsilon$ on $\partial\Omega\cap B_\rho(x_0)$. On the rest of the boundary, $-g\geq m\rho^\nu$. The boundary is [compact](../../../../../../compact-space.md), so $\varphi$ is bounded. Choose $A>0$ large enough that $A\delta\geq M$ and

$$
A(-g(x))\geq|\varphi(x)-\varphi(x_0)|
\quad\text{on }\partial\Omega\setminus B_\rho(x_0).
$$

Then the [Perron subfunction for the Poisson equation](../../../../../../perron-subfunction-for-the-poisson-equation.md) and its superfunction counterpart

$$
v_-(x)=\varphi(x_0)-\varepsilon+Ag(x),\qquad
v_+(x)=\varphi(x_0)+\varepsilon-Ag(x)
$$

satisfy $\Delta v_-\geq M\geq f$, $\Delta v_+\leq-M\leq f$, and $v_-\leq\varphi\leq v_+$ on the whole boundary. The near-boundary ordering uses the choice of $\rho$; the remaining ordering uses the choice of $A$. In particular the Perron family is nonempty and bounded above.

The [Perron method for the Dirichlet problem](../../../../../../perron-method.md) and the permitted comparison give $v_-\leq u\leq v_+$. Since $g(x)\to0$ as $x\to x_0$, we obtain

$$
\varphi(x_0)-\varepsilon\leq\liminf_{x\to x_0}u(x)
\leq\limsup_{x\to x_0}u(x)\leq\varphi(x_0)+\varepsilon.
$$

Letting $\varepsilon\downarrow0$ proves

$$
\boxed{\lim_{\Omega\ni x\to x_0}u(x)=\varphi(x_0).}
$$

The interior Perron theorem gives [continuity](../../../../../../continuous-function.md) inside $\Omega$, and the displayed limit together with [continuity](../../../../../../continuous-function.md) of $\varphi$ proves **the continuous extension $u\in C^0(\overline\Omega)$ with the required boundary trace**. Thus every boundary point is a [regular boundary point](../../../../../../regular-boundary-point.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
