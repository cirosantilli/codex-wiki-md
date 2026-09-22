<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

It is equivalent to minimize $\|z\|_q$ or its $q$th power $F_q(z)=\sum_i|z_i|^q$, because taking the $q$th root is strictly increasing. For $q<1$, this is an [Lq quasi-norm](../../../../../../lq-quasi-norm.md), while $q=1$ gives the [L1 norm](../../../../../../l1-norm.md).

Assume the [Lq null space property](../../../../../../lq-null-space-property.md) of order $s$. Let $x$ have [support of a vector](../../../../../../support-of-a-vector.md) $S$ with $|S|\le s$, and let $z=x+v$ be any distinct feasible [vector](../../../../../../vector.md). Then $0\ne v\in\ker A$. The [triangle inequality](../../../../../../triangle-inequality.md) for complex magnitudes and the subadditivity $(a+b)^q\le a^q+b^q$ give

$$
|x_i|^q\le(|x_i+v_i|+|v_i|)^q\le|x_i+v_i|^q+|v_i|^q.
$$

For $q=1$ the same inequality follows directly from the [triangle inequality](../../../../../../triangle-inequality.md). Since $x=0$ off $S$,

$$
F_q(x+v)\ge F_q(x)-\sum_{i\in S}|v_i|^q+\sum_{i\notin S}|v_i|^q>F_q(x).
$$

Thus $x$ is the unique minimizer.

Conversely, suppose every $s$-sparse [vector](../../../../../../vector.md) is the unique minimizer for its measurements. Fix $0\ne v\in\ker A$ and any $S$ with $|S|\le s$. The [vectors](../../../../../../vector.md) $x=-v_S$ and $z=v_{S^c}$ are distinct and satisfy $Az=Ax$, since $Av=0$. Uniqueness for this $x$ therefore implies $F_q(x)<F_q(z)$, exactly the required strict inequality. Hence

$$
\boxed{\text{uniform unique }s\text{-sparse }\ell^q\text{ recovery}\ \Longleftrightarrow\ \sum_{i\in S}|v_i|^q<\sum_{i\notin S}|v_i|^q\quad(0\ne v\in\ker A,\ |S|\le s).}
$$

The quantifier is uniform over the entire sparse class. Recovery of one particular signed [vector](../../../../../../vector.md) alone would not imply this [null space property](../../../../../../nullspace-property.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
