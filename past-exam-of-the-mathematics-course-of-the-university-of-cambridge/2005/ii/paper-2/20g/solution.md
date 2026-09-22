<h1 id="20g/solution">Solution</h1>

↑ **Parent:** [20G](../20g.md)

The [ring of integers](../../../../../ring-of-integers.md) is $\mathcal O_k=\mathbb Z[\sqrt7]$, since $7\equiv3\pmod4$, and its [discriminant](../../../../../discriminant.md) is $28$. Rationalizing gives

$$
\varepsilon=8+3\sqrt7,\qquad\varepsilon^{-1}=8-3\sqrt7,\qquad N(\varepsilon)=1.
$$

Both are algebraic integers, so **$\varepsilon$ is a [unit](../../../../../unit-in-a-ring.md)**. Set $\mathfrak p=(3+\sqrt7)$. Since $(3+\sqrt7)^2=2\varepsilon$,

$$
\boxed{\mathfrak p^2=(2).}
$$

Also $N(\mathfrak p)=|N(3+\sqrt7)|=2$. It is the unique ideal of [ideal norm](../../../../../ideal-norm.md) two: any quotient of size two is $\mathbb F_2$, and the image of $\sqrt7$ must satisfy $z^2=1$, hence be one. The [kernel of a ring homomorphism](../../../../../kernel-of-a-ring-homomorphism.md) onto $\mathbb F_2$ is uniquely $(2,1+\sqrt7)$, which is $\mathfrak p$.

The given Minkowski constant means every [ideal class](../../../../../ideal-class.md) has an integral representative of [ideal norm](../../../../../ideal-norm.md) at most $\frac12\sqrt{28}=\sqrt7<3$. Such a [ideal norm](../../../../../ideal-norm.md) is one or two. The norm-one ideal is the whole ring, and the sole norm-two ideal is principal. Thus **the [class number](../../../../../class-number.md) is one**.

If $x^2-7y^2=2$, the [principal ideal](../../../../../principal-ideal.md) $(x+y\sqrt7)$ has [ideal norm](../../../../../ideal-norm.md) two and hence equals $\mathfrak p$. Its generator differs from $3+\sqrt7$ by a [unit](../../../../../unit-in-a-ring.md). Conversely multiplication by a norm-one [unit](../../../../../unit-in-a-ring.md) preserves the [field norm](../../../../../field-norm.md) two. With the assumed [fundamental unit](../../../../../fundamental-unit-number-theory.md), all [units](../../../../../unit-in-a-ring.md) are $\pm\varepsilon^n$; in fact a norm-minus-one [unit](../../../../../unit-in-a-ring.md) is impossible since $x^2\equiv-1\pmod7$ has no solution. Therefore the complete answer is

$$
\boxed{x+y\sqrt7=\pm(8+3\sqrt7)^n(3+\sqrt7),\qquad n\in\mathbb Z.}
$$

For $n=1$ and the positive sign, the product is $45+17\sqrt7$, giving **$(x,y)=(45,17)$**; $45^2-7\cdot17^2=2$ checks the result.

## ↑ Ancestors (10)

1. [20G](../20g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
