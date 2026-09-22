<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $S=\operatorname{supp}x$ be the [support of a vector](../../../../../../support-of-a-vector.md) $x$, with $|S|\le s$. Suppose the [null space property](../../../../../../nullspace-property.md) holds. Every other feasible [vector](../../../../../../vector.md) is $z=x+v$, where $0\ne v\in\ker A$. Splitting its [L1 norm](../../../../../../l1-norm.md) over $S$ and $S^c$ and using the [triangle inequality](../../../../../../triangle-inequality.md) gives

$$
\|x+v\|_1=\|x_S+v_S\|_1+\|v_{S^c}\|_1\ge\|x\|_1-\|v_S\|_1+\|v_{S^c}\|_1>\|x\|_1.
$$

Thus the [sparse vector](../../../../../../sparse-vector.md) $x$ is the unique [minimizer](../../../../../../global-minimizer.md) in [basis pursuit](../../../../../../basis-pursuit.md). Notice that the argument works for complex coordinates: it uses the [absolute value](../../../../../../absolute-value.md) inequality, rather than a real [sign function](../../../../../../sign-function.md).

Conversely, suppose [basis pursuit](../../../../../../basis-pursuit.md) uniquely recovers every [sparse vector](../../../../../../sparse-vector.md) of order $s$. Fix $0\ne v\in\ker A$ and any $S$ with $|S|\le s$. Take $x=-v_S$ and $z=v_{S^c}$. These [vectors](../../../../../../vector.md) have the same measurements, because $Av_S+Av_{S^c}=0$, and they are distinct since $z-x=v\ne0$. The [vector](../../../../../../vector.md) $x$ has at most $s$ nonzero coordinates, so uniqueness gives

$$
\|v_S\|_1=\|x\|_1<\|z\|_1=\|v_{S^c}\|_1.
$$

This is the [null space property](../../../../../../nullspace-property.md) for every such $S$. **Uniform unique recovery by [basis pursuit](../../../../../../basis-pursuit.md) is equivalent to the order-$s$ [null space property](../../../../../../nullspace-property.md).**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
