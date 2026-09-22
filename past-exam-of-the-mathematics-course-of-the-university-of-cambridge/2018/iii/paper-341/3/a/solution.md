<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The original PDF puts both neighbouring values at time $n+1$. Thus the actual scheme is [Backward Euler method](../../../../../../backward-euler-method.md) in time with a centered three-point approximation to the second spatial derivative. The old-time neighbours in the TeX transcription describe a different method.

Let $h=\Delta x$ and $k=\Delta t$. Insert a sufficiently smooth exact solution and divide by $k$. Expanding at $(x_m,t_{n+1})$ gives

$$
\frac{u(x_m,t_{n+1})-u(x_m,t_n)}k
-\frac{u(x_m-h,t_{n+1})-2u(x_m,t_{n+1})+u(x_m+h,t_{n+1})}{h^2}
=-\frac{k}{2}u_{tt}-\frac{h^2}{12}u_{xxxx}+O(k^2+h^4).
$$

The PDE cancels the $u_t-u_{xx}$ term. Therefore the normalized [local truncation error](../../../../../../local-truncation-error.md) is $O(k+h^2)$ and

$$
\boxed{\text{first order in time and second order in space}.}
$$

For compatible smooth data with exact nodal initialization, the [stability of a numerical method](../../../../../../stability-of-a-numerical-method.md) established below gives [global error](../../../../../../global-discretization-error.md) $O(k+h^2)$ on fixed time intervals, by summing the one-step defects with the contraction bound. Thus no relation between $k$ and $h$ is needed for stability; choosing $k=O(h^2)$ makes both consistency contributions $O(h^2)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
