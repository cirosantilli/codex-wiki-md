<h1 id="18h/solution">Solution</h1>

↑ **Parent:** [18H](../18h.md)

The [Artin fixed-field theorem](../../../../../artin-fixed-field-theorem.md) says that for a finite group $G$ of distinct automorphisms of a field $K$, the extension $K/K^G$ is [Galois extension](../../../../../finite-galois-extension.md) and has degree $|G|$. Here $y=x^p-x$ is invariant under translations because $(x+a)^p-(x+a)=x^p-x$ for $a\in\mathbb F_p$. Hence $\mathbb F_p(y)\subset K^G$. Also $x$ is a root of $T^p-T-y$, so $[K:\mathbb F_p(y)]\le p$. The fixed-field theorem gives $[K:K^G]=p$, forcing $\boxed{K^G=\mathbb F_p(y)}$. The extension is [separable](../../../../../separable-topological-space.md); explicitly the derivative of $T^p-T-y$ is $-1$.

For the affine substitutions, $y$ transforms to $dy$, since $d^p=d$ and $a^p=a$. Therefore $z=y^{p-1}$ is fixed by all $p(p-1)$ substitutions. The polynomial $(T^p-T)^{p-1}-z$ has $x$ as a root and degree $p(p-1)$. Apply the same degree comparison and the [Artin fixed-field theorem](../../../../../artin-fixed-field-theorem.md) to obtain

$$
\boxed{K^H=\mathbb F_p(z),\qquad z=(x^p-x)^{p-1}.}
$$

Moreover $[\mathbb F_p(y):\mathbb F_p(z)]=p-1$, so the [minimal polynomial](../../../../../minimal-polynomial.md) of $y$ is $\boxed{T^{p-1}-z}$. It splits as $\prod_{d\in\mathbb F_p^\times}(T-dy)$, and its derivative is nonzero at every root. Thus $K^G/K^H$ is a [Galois extension](../../../../../finite-galois-extension.md) with group $\mathbb F_p^\times$, acting by $y\mapsto dy$.

There is a harmless convention issue in labeling the substitutions: $f(x)\mapsto f(dx+a)$ composes in the reverse order to the displayed affine matrices. It is naturally a right action on functions, or a left action after inserting inverses. The set of automorphisms and all the [fixed fields](../../../../../fixed-field.md) just computed are unchanged by that convention.

## ↑ Ancestors (10)

1. [18H](../18h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
