<h1 id="5a/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Impose the target temperature on the post-jump [exponential decay](../../../../../../../exponential-decay.md):

$$
\left[\left(\frac\alpha2-1\right)T_0+\beta\right]e^{-k(t_2-t_1)}=(\alpha-1)T_0.
$$

Solving for the jump and eliminating $t_1$ using $e^{kt_1}=2(\alpha-1)/(\alpha-2)$ gives

$$
\boxed{\beta=(\alpha-1)T_0e^{k(t_2-t_1)}-\frac{\alpha-2}{2}T_0=\frac{\alpha-2}{2}T_0\bigl(e^{kt_2}-1\bigr).}
$$

**This is the unique required temperature increase, and it satisfies the stipulated lower bound.** Indeed $t_2>t_1$ implies

$$
\beta-\frac{\alpha T_0}{2}=(\alpha-1)T_0\bigl(e^{k(t_2-t_1)}-1\bigr)>0.
$$

Thus no additional restriction on the prescribed time is needed.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [5A](../../../5a.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ia](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
