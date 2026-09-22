<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\alpha=\sqrt[3]{3}$. The [polynomial](../../../../polynomial-split.md) $X^3-3$ is [Eisenstein](../../../../eisenstein-criterion.md) at three, so the [number field](../../../../number-field.md) has [degree of a field extension](../../../../degree-of-a-field-extension.md) three. Use the permitted [ring of integers](../../../../ring-of-integers.md) $R=\mathbb Z[\alpha]$, whose [integral basis](../../../../integral-basis.md) is $1,\alpha,\alpha^2$. The [field traces](../../../../field-trace.md) $\operatorname{Tr}(1)=3$, $\operatorname{Tr}(\alpha)=\operatorname{Tr}(\alpha^2)=0$, $\operatorname{Tr}(\alpha^3)=9$, and $\operatorname{Tr}(\alpha^4)=0$ give

$$
d_K=\det\begin{pmatrix}3&0&0\\0&0&9\\0&9&0\end{pmatrix}=-243.
$$

There is one real [field embedding](../../../../field-embedding.md) and one conjugate pair of nonreal [field embeddings](../../../../field-embedding.md). The [Minkowski bound for ideal classes](../../../../minkowski-s-bound.md) is therefore

$$
\frac4\pi\frac{3!}{3^3}\sqrt{243}=\frac{8\sqrt3}{\pi}<5.
$$

Every [ideal class](../../../../ideal-class.md) has an [integral ideal](../../../../integral-ideal.md) representative of [ideal norm](../../../../ideal-norm.md) at most four, so it is enough to show that every [prime ideal](../../../../prime-ideal.md) of [ideal norm](../../../../ideal-norm.md) at most four is a [principal ideal](../../../../principal-ideal.md).

Modulo two,

$$
X^3-3\equiv(X+1)(X^2+X+1),
$$

where the quadratic factor is an [irreducible polynomial](../../../../irreducible-polynomial.md) over the [finite field](../../../../finite-field.md) $\mathbb F_2$. The [Dedekind factorization theorem](../../../../dedekind-factorization-theorem.md) gives

$$
(2)=P_2Q_2,\quad P_2=(2,\alpha-1),\quad N(P_2)=2,\quad
Q_2=(2,\alpha^2+\alpha+1),\quad N(Q_2)=4.
$$

Now

$$
N_{K/\mathbb Q}(\alpha-1)=2,
\qquad (\alpha-1)(\alpha^2+\alpha+1)=2.
$$

Thus $(\alpha-1)=P_2$, by containment and equality of [ideal norms](../../../../ideal-norm.md), and cancellation in the second identity gives $(\alpha^2+\alpha+1)=Q_2$. This explicitly handles the [prime ideal](../../../../prime-ideal.md) of [ideal norm](../../../../ideal-norm.md) four, as well as the one of [ideal norm](../../../../ideal-norm.md) two.

Modulo three the [polynomial](../../../../polynomial-split.md) is $X^3$, so

$$
(3)=P_3^3,\qquad P_3=(3,\alpha)=(\alpha),\qquad N(P_3)=3.
$$

These exhaust the [prime ideals](../../../../prime-ideal.md) of [ideal norm](../../../../ideal-norm.md) at most four. Every bounded representative factors into the listed [principal ideals](../../../../principal-ideal.md), and hence is a [principal ideal](../../../../principal-ideal.md). Therefore the [Class group of Q of cube root of three](../../../../class-group-of-q-of-cube-root-of-three.md) is

$$
\boxed{\operatorname{Cl}(\mathbb Q(\sqrt[3]{3}))=1}.
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the algebraic number theory course of the University of Oxford](../../../split.md)
5. [Algebraic number theory course of the University of Oxford](../../../../algebraic-number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
