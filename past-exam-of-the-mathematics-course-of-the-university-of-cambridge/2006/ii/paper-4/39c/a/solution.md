<h1 id="39c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $h=\Delta x$, $k=\Delta t$ and apply the recurrence to an exact smooth solution. The centred second difference is $h^2u_{xx}+h^4u_{xxxx}/12+O(h^6)$. Expanding the previous-time second difference and using $u_t=u_{xx}$ gives the one-step residual

$$
\begin{aligned}
&u(t+k)-u(t)-\tfrac32\mu\delta_h^2u(t)+\tfrac12\mu\delta_h^2u(t-k)\\
&=\frac{k^2}{2}(u_{tt}-u_{xxt})-\frac{kh^2}{12}u_{xxxx}
+O(k^3+k^2h^2+kh^4)\\
&=-\frac{k^2}{12\mu}u_{xxxx}+O(k^3),
\end{aligned}
$$

where $h^2=k/\mu$ with fixed positive $\mu$. Thus **the local one-step error is $O((\Delta t)^2)$** as stated. If [local truncation error](../../../../../../local-truncation-error.md) is defined after division by the step, it is instead $O(\Delta t)$ in this coupled refinement; the spatial error is only second order in $h$. This distinguishes the printed local-error convention from the second-order time accuracy of the underlying [Adams-Bashforth method](../../../../../../adams-bashforth-method.md) at fixed spatial discretization.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [39C](../../39c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
