<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For $0\leq x\leq B$, the two variational comparisons agree. Outside that interval the finite-buffer fiber is empty, since its [queue workload](../../../../../../workload-of-a-queue.md) always lies in $[0,B]$. The [finite-buffer workload rate truncation](../../../../../../finite-buffer-workload-rate-truncation.md) is therefore

$$
\boxed{\bar J(x)=\begin{cases}J(x),&0\leq x\leq B,\\\infty,&x<0\text{ or }x>B.\end{cases}}
$$

Equivalently this is J for $x\leq B$ and infinity above B, since J already assigns infinity to negative [queue workloads](../../../../../../workload-of-a-queue.md). Together with the contracted LDP from the first part, this proves the requested principle. The rate is good by contraction; alternatively its finite [sublevel sets](../../../../../../sublevel-set.md) are the [compact sets](../../../../../../compact-space.md) $\{J\leq M\}\cap[0,B]$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
