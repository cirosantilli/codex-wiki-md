<h1 id="16i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A finite [field extension](../../../../../../field-extension.md) $L/K$ is a [separable field extension](../../../../../../separable-extension.md) if every element of $L$ has a [minimal polynomial](../../../../../../minimal-polynomial.md) over $K$ with distinct roots in an [algebraic closure](../../../../../../algebraic-closure.md). The [primitive element theorem](../../../../../../primitive-element-theorem.md) says that a finite [separable field extension](../../../../../../separable-extension.md) $L/K$ is $K(\alpha)$ for some $\alpha\in L$.

If $K$ is finite, then so is $L$. The multiplicative group of a [finite field](../../../../../../finite-field.md) is cyclic, so a generator of $L^\times$ generates $L$ as a field. To justify the group fact, a finite subgroup of a field's multiplicative group is cyclic: in a [finite abelian group](../../../../../../finite-abelian-group.md) its exponent is attained as an element order, while the [polynomial](../../../../../../polynomial-split.md) root bound forces its size to be at most that exponent.

If $K$ is infinite, first consider $L=K(a,b)$. The [minimal polynomials](../../../../../../minimal-polynomial.md) of $a$ and $b$ have distinct roots $a_i,b_j$ in an [algebraic closure](../../../../../../algebraic-closure.md). Choose $c\in K$, $c\ne0$, avoiding the finitely many values for which $a_i+cb_j=a+cb$ for a pair other than $(a,b)$. Set $\alpha=a+cb$. Over $K(\alpha)$, the [polynomials](../../../../../../polynomial-split.md) $f(T)$ and $g((\alpha-T)/c)$ have precisely one common root, $a$. Their monic [greatest common divisor](../../../../../../greatest-common-divisor.md) is therefore $T-a$, so $a\in K(\alpha)$ and $b=(\alpha-a)/c\in K(\alpha)$. Thus $K(a,b)=K(\alpha)$. Induct over finitely many generators of the finite [separable field extension](../../../../../../separable-extension.md). This proves **every finite separable extension is simple**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16I](../../16i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
