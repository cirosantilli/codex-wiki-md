<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First the [null space property](../../../../../../nullspace-property.md) implies [sparse injectivity](../../../../../../sparse-injectivity.md). If a nonzero $v\in\ker A$ had at most $2s$ nonzero coordinates, partition its [support of a vector](../../../../../../support-of-a-vector.md) into disjoint $S,T$ with $|S|,|T|\le s$. Applying the [null space property](../../../../../../nullspace-property.md) to each of these sets yields

$$
\|v_S\|_1<\|v_T\|_1\quad\hbox{and}\quad\|v_T\|_1<\|v_S\|_1,
$$

which is impossible. Hence the [null space](../../../../../../kernel-of-a-linear-map.md) contains no nonzero [sparse vector](../../../../../../sparse-vector.md) of order $2s$.

The feasible [vector](../../../../../../vector.md) $x$ has $\|x\|_0\le s$, where the [L0 sparsity count](../../../../../../l0-sparsity-count.md) counts its nonzero coordinates. Any different feasible $z$ with $\|z\|_0\le\|x\|_0$ would give a nonzero [null space](../../../../../../kernel-of-a-linear-map.md) [vector](../../../../../../vector.md) $z-x$ with at most $2s$ nonzero coordinates, contrary to [sparse injectivity](../../../../../../sparse-injectivity.md). Consequently every different feasible $z$ has strictly larger [L0 sparsity count](../../../../../../l0-sparsity-count.md). **The unique sparsest feasible vector is $x$:**

$$
\boxed{\operatorname*{arg\,min}_{Az=Ax}\|z\|_0=\{x\}.}
$$

This proof does not treat the [L0 sparsity count](../../../../../../l0-sparsity-count.md) as a genuine [norm](../../../../../../norm.md); no [triangle inequality](../../../../../../triangle-inequality.md) for it is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
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
