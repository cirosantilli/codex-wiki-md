<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Interpret the [normal-operator source condition](../../../../../../normal-operator-source-condition.md) as the displayed intersection condition: there is $v\in U$ with $w=K^*Kv\in\partial J(u^\dagger)$. Fix any $\alpha>0$ and put $\bar u=u^\dagger+\alpha v$. The [subgradient optimality condition](../../../../../../subgradient-optimality-condition.md) for the artificial-data objective is

$$
0\in K^*(Ku^\dagger-K\bar u)+\alpha\partial J(u^\dagger).
$$

It holds because its first term equals $-\alpha K^*Kv=-\alpha w$. By [convexity](../../../../../../convex-function.md), this is sufficient for global minimality, proving the forward implication. Conversely, if $u^\dagger$ minimizes that objective, the same optimality condition gives

$$
w=\frac1\alpha K^*K(\bar u-u^\dagger)\in\partial J(u^\dagger).
$$

Taking $v=(\bar u-u^\dagger)/\alpha$ proves the intersection condition. Thus **the two conditions are equivalent when the source vector is allowed to be zero**.

The printed additional requirement $v\ne0$ is not equivalent in general. For $K=I$ and $J\equiv0$, the displayed source condition holds, and choosing $\bar u=u^\dagger$ makes $u^\dagger$ the minimizer, but $\partial J(u^\dagger)=\{0\}$ forces $v=0$. A nonzero-source version needs an additional hypothesis, such as requiring $w\ne0$; it cannot be inferred from the printed intersection alone.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
