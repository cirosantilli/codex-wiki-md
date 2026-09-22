<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $u=A^*h$ be the [strict dual certificate for basis pursuit](../../../../../../strict-dual-certificate-for-basis-pursuit.md) supplied by condition (ii). For $0\ne v\in\ker A$, we have

$$
0=\langle h,Av\rangle=\langle A^*h,v\rangle=\langle\operatorname{sgn}(x_S),v_S\rangle+\sum_{l\in S^c}u_l v_l.
$$

Here the [adjoint operator](../../../../../../adjoint-operator.md) is the real transpose. The [injectivity](../../../../../../injective-function.md) of $A_S$ ensures $v_{S^c}\ne0$: otherwise $A_Sv_S=0$ would force $v=0$. Thus at least one nonzero term lies outside the [support of a vector](../../../../../../support-of-a-vector.md) $x$. Since $|u_l|<1$ at every such index,

$$
|\langle\operatorname{sgn}(x_S),v_S\rangle|=\left|\sum_{l\in S^c}u_l v_l\right|\le\sum_{l\in S^c}|u_l|\,|v_l|<\sum_{l\in S^c}|v_l|.
$$

This proves the [fixed-sign null space condition](../../../../../../fixed-sign-null-space-condition.md), so part (a) gives uniqueness in [basis pursuit](../../../../../../basis-pursuit.md). If $S^c$ is empty, the [injectivity](../../../../../../injective-function.md) of $A_S=A$ instead means there is no nonzero [null space](../../../../../../kernel-of-a-linear-map.md) [vector](../../../../../../vector.md), and the feasible set is a singleton. **[Injective](../../../../../../injective-function.md) active columns and a [strict dual certificate for basis pursuit](../../../../../../strict-dual-certificate-for-basis-pursuit.md) ensure unique recovery.** Both ingredients matter: strictness outside $S$ cannot detect a nonzero [null space](../../../../../../kernel-of-a-linear-map.md) direction supported entirely inside $S$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
