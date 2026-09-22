<h1 id="28l/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

While the queue is nonempty, service completions occur at rate $\mu$. A completion reduces the queue length only when the customer leaves, which has probability $1-p$. Thinning therefore makes $L$ a birth--death chain with birth rate

$$
\lambda
$$

and effective death rate

$$
\delta=\mu(1-p).
$$

The standard birth--death classification gives

$$
\boxed{
L\text{ is transient if }\lambda>\mu(1-p),
\quad
L\text{ is recurrent if }\lambda\leq\mu(1-p).}
$$

At equality it is null recurrent.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [28L](../../../28l.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
