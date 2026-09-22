<h1 id="30c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $w$ be the difference between a $C^2$ solution and the formula in part (ii). It satisfies $w_{tt}-\Delta w=0$ and zero initial data. Fix $(T,x_0)$ and $\varepsilon>0$, and put $B_t=B(x_0,T+\varepsilon-t)$. Define the local energy

$$
E(t)=\frac12\int_{B_t}(w_t^2+|\nabla w|^2)\,dx.
$$

Differentiating on the shrinking ball and integrating by parts gives

$$
E'(t)=\int_{\partial B_t}\left[w_t\partial_nw-\tfrac12(w_t^2+|\nabla w|^2)\right]dS\leq0,
$$

since $2w_t\partial_nw\leq w_t^2+(\partial_nw)^2\leq w_t^2+|\nabla w|^2$. Initially $E=0$, hence $w_t=\nabla w=0$ inside each ball. In particular $w(t,x_0)$ is constant from its initial value zero, so $w(T,x_0)=0$. Since the point was arbitrary, **every $C^2$ solution equals the Kirchhoff solution**. This [shrinking cone energy argument](../../../../../../shrinking-cone-energy-argument.md) uses only energy on compact sets, so it does not assume global decay of the competing solution.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [30C](../../30c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
