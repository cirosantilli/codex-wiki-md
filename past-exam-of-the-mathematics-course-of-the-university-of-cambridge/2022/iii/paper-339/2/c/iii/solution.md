<h1 id="2/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

When $A$ has full row rank, projected gradient ascent with step $1/L$ has linear convergence and requires

$$
\boxed{k=O\left(\frac L\mu\log\frac1\epsilon\right)}
$$

iterations, up to the initial-error constant. The accelerated projected method of [Nesterov](../../../../../../../nesterov-accelerated-gradient-method.md) requires

$$
\boxed{k=O\left(\sqrt{\frac L\mu}\log\frac1\epsilon\right).}
$$

Without full row rank, the general smooth-convex bounds are $O(LR^2/\epsilon)$ and $O(\sqrt{LR^2/\epsilon})$, respectively, when a dual optimum lies within distance $R$ of the initial point.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 339](../../../../paper-339-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
