<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $c=\sqrt{g'h}$. The three real eigenvalues are

$$
\boxed{\lambda_0=u,\qquad\lambda_\pm=u\pm c},
$$

so the system is strictly hyperbolic for $g'h>0$. Along $dx/dt=u$,

$$
\boxed{\frac{D_0g'}{Dt}=-g'\frac{w_e}{h}}.
$$

Left eigenvectors for $\lambda_\pm$ are $(\pm h/(2c),\pm c/h,1)$, hence

$$
\boxed{
D_\pm u\pm\frac chD_\pm h\pm\frac h{2c}D_\pm g'
=\pm\frac ch\left(\frac{w_e}{2}-w_d\right)-u\frac{w_e}{h}},
$$

where $D_\pm=\partial_t+(u\pm c)\partial_x$.

When $w_e,w_d\to0$, reduced gravity is materially conserved. If it is initially uniform, it remains constant and the other two relations integrate to the standard [Riemann invariants](../../../../../../riemann-invariant.md)

$$
\boxed{D_\pm(u\pm2\sqrt{g'h})=0}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
