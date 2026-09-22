<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

With $n$ individuals, each of the $n$ can reproduce at rate $\lambda$ and independently die at rate $\lambda$. Thus the total birth and death rates are $q_n=r_n=\lambda n$. The gain into state $n$ comes from a birth in state $n-1$ and a death in state $n+1$, while its loss rate is $2\lambda n$. Therefore

$$
\boxed{\dot P_n=\lambda(n-1)P_{n-1}+\lambda(n+1)P_{n+1}-2\lambda nP_n.}
$$

At $n=0$, the birth inflow from negative states is absent and $\dot P_0=\lambda P_1$. The empty state is absorbing: once the population reaches zero, neither process can restart it. Equal birth and death rates make this a [critical branching process](../../../../critical-branching-process.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
