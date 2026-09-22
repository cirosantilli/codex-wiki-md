<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [Qp-Banach algebra](../../../../../qp-banach-algebra.md) is a $\mathbb Q_p$-algebra with a complete non-Archimedean submultiplicative norm compatible with the [p-adic absolute value](../../../../../p-adic-absolute-value.md). A p-valued group is [p-saturated](../../../../../p-saturated-group.md) when it is complete and every $g$ with $\omega(g)>p/(p-1)$ has a pth root.

In the completed rational Iwasawa algebra $\widehat{\mathbb Q_pG}$, the filtration of $g-1$ is $\omega(g)>1/(p-1)$. Since $v_p(n)=O(\log n)$, the terms of

$$
\log g=\sum_{n\geq1}\frac{(-1)^{n+1}}n(g-1)^n
$$

have filtrations tending to infinity, so the series converges. The [Baker--Campbell--Hausdorff formula](../../../../../baker-campbell-hausdorff-formula.md) expresses $\log(gh)$ in terms of $\log g$ and $\log h$, and its commutator expansion expresses $\log([g,h])$ with leading term $[\log g,\log h]$. Completeness and p-divisibility allow the higher terms to be removed successively. Integer powers give $\log(g^n)=n\log g$, and continuity extends scalar multiplication to $\mathbb Z_p$. Thus the [Lazard logarithm of a p-saturated group](../../../../../lazard-logarithm-of-a-p-saturated-group.md) shows that $\log(G)$ is a $\mathbb Z_p$-Lie subalgebra.

The group-like coproduct identity $\Delta(g)=g\otimes g$ implies

$$
\Delta(\log g)=\log g\otimes1+1\otimes\log g,
$$

so each logarithm is primitive. If $(g_1,\ldots,g_d)$ is an ordered basis, their initial forms are linearly independent. Conversely, for a primitive element, its lowest initial form must be linear rather than a product; subtracting a $\mathbb Q_p$-linear combination of the $\log(g_i)$ raises its filtration. Iteration and completeness leave zero. Hence the [primitive elements of a completed rational Iwasawa algebra](../../../../../primitive-elements-of-a-completed-rational-iwasawa-algebra.md) satisfy

$$
\boxed{P(\widehat{\mathbb Q_pG})
=\bigoplus_{i=1}^d\mathbb Q_p\log(g_i).}
$$

For the upper-triangular group, ordinary matrix logarithms give

$$
\log\begin{pmatrix}1+a&b\\0&1\end{pmatrix}
=\begin{pmatrix}
\log(1+a)&b\,\dfrac{\log(1+a)}a\\[4pt]
0&0
\end{pmatrix},
$$

with the quotient interpreted as $1$ at $a=0$. For odd $p$, both $a\mapsto\log(1+a)$ and $a\mapsto\log(1+a)/a$ are respectively a bijection $p\mathbb Z_p\to p\mathbb Z_p$ and a unit-valued function. Therefore

$$
\boxed{\log(G)=
\left\{\begin{pmatrix}u&v\\0&0\end{pmatrix}:u,v\in p\mathbb Z_p\right\}.}
$$

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 145](../../paper-145-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
