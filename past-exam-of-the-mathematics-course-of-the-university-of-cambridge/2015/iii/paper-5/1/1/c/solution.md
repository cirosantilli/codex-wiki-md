<h1 id="1/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the same formula for a measurable representative of $u_0$. Dilation preserves null sets and gives $\|u\|_{L^\infty}=\|u_0\|_{L^\infty}$. To check the [weak formulation](../../../../../../../weak-formulation.md), change variables $x=e^t y$ and set $\psi(t,y)=e^t\varphi(t,e^t y)$. Then

$$
e^t(\varphi_t+x\varphi_x+\varphi)(t,e^t y)=\psi_t(t,y).
$$

The spacetime integral becomes $\int u_0(y)\psi_t(t,y)\,dy\,dt=-\int u_0(y)\varphi(0,y)\,dy$, as required.

For uniqueness, take any bounded [weak solution](../../../../../../../weak-solution.md) and write $v(t,y)=u(t,e^t y)$. Choosing $\varphi(t,x)=e^{-t}\psi(t,e^{-t}x)$ in the [weak formulation](../../../../../../../weak-formulation.md) gives

$$
\int v\psi_t\,dy\,dt+\int u_0(y)\psi(0,y)\,dy=0.
$$

For tensor [test functions](../../../../../../../test-function.md) $\psi(t,y)=\eta(t)\theta(y)$, this says that $\int v(t,y)\theta(y)\,dy$ is distributionally constant and has value $\int u_0\theta$. A countable dense family of spatial [test functions](../../../../../../../test-function.md) identifies $v=u_0$ [almost everywhere](../../../../../../../almost-everywhere.md). Thus **the displayed solution is the unique bounded weak solution**.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
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
