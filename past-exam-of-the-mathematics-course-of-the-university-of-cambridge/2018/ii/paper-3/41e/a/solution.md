<h1 id="41e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\delta_x^2u_m=u_{m-1}-2u_m+u_{m+1}$. For an exact smooth solution of the [diffusion equation](../../../../../../diffusion-equation-split.md), the [second-order central difference](../../../../../../second-order-central-difference.md) gives

$$
\delta_x^2u(x,t)=h^2u_{xx}(x,t)+\frac{h^4}{12}u_{xxxx}(x,t)+O(h^6).
$$

Since the [Courant number](../../../../../../courant-number.md) $\mu=k/h^2$ is fixed, $h^2=O(k)$. Taylor expansion in time gives

$$
\begin{aligned}
u(t+k)-u(t)&=ku_t+\frac{k^2}{2}u_{tt}+O(k^3),\\
\frac32\mu\delta_x^2u(t)-\frac12\mu\delta_x^2u(t-k)
&=ku_{xx}+\frac{k^2}{2}u_{xxt}+O(kh^2)+O(k^3).
\end{aligned}
$$

Using $u_t=u_{xx}$ and $u_{tt}=u_{xxt}$ cancels the leading terms. Because $kh^2=O(k^2)$, the residual, and hence the [local truncation error](../../../../../../local-truncation-error.md) in the convention of the question, is

$$
\boxed{O(k^2).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [41E](../../41e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
