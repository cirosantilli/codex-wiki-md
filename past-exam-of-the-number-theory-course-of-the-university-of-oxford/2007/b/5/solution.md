<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For the $n$ distinct complex embeddings $\sigma_1,\ldots,\sigma_n$ of the [number field](../../../../number-field.md), define the [discriminant of elements of a number field](../../../../discriminant-of-elements-of-a-number-field.md) by

$$
D(w_1,\ldots,w_n)=\det(\sigma_i(w_j))^2
=\det\bigl(\operatorname{Tr}_{K/\mathbb Q}(w_iw_j)\bigr).
$$

The equality follows by multiplying the transpose of the embedding [matrix](../../../../matrix.md) by itself. Each [field trace](../../../../field-trace.md) is rational: it is also the trace of the rational [matrix](../../../../matrix.md) of multiplication by $w_iw_j$ on $K$. Thus the [determinant](../../../../determinant.md) lies in $\mathbb Q$. If the $w_i$ are [algebraic integers](../../../../algebraic-integer.md), the products and their conjugates are [algebraic integers](../../../../algebraic-integer.md), and so are their sums. A rational [algebraic integer](../../../../algebraic-integer.md) is an [integer](../../../../integer-split.md), hence all trace entries and their [determinant](../../../../determinant.md) are [integers](../../../../integer-split.md).

Write $u_j=\sum_i a_{ij}v_i$. The inclusion of the generated abelian [groups](../../../../group-split.md) makes $A=(a_{ij})$ an [integer](../../../../integer-split.md) [matrix](../../../../matrix.md). Its embedding [matrix](../../../../matrix.md) is the embedding [matrix](../../../../matrix.md) of the $v_i$ multiplied by $A$. Taking squared [determinants](../../../../determinant.md) gives

$$
\boxed{D(u_1,\ldots,u_n)=(\det A)^2D(v_1,\ldots,v_n).}
$$

For independent [algebraic integers](../../../../algebraic-integer.md) $v_i$, choose an [integral basis](../../../../integral-basis.md) $\omega_i$ of $\mathcal O_K$. The same formula gives $D(v)=[\mathcal O_K:\sum_i\mathbb Zv_i]^2D(\omega)$. If $D(v)$ is nonzero and a [square-free integer](../../../../square-free-integer.md), the [integer](../../../../integer-split.md) index must be one, proving that the $v_i$ form an [integral basis](../../../../integral-basis.md).

Now put $\beta=3\alpha+4$. Since $\mathbb Q(\beta)=\mathbb Q(\alpha)$ has degree three, the [monic polynomial](../../../../monic-polynomial.md)

$$
27f\!\left(\frac{X-4}{3}\right)=X^3-6X^2+59
$$

is its [minimal polynomial of an algebraic element](../../../../minimal-polynomial-of-an-algebraic-element.md). The [field norm](../../../../field-norm.md) is the negative of its constant term:

$$
\boxed{\operatorname{Norm}_{K/\mathbb Q}(3\alpha+4)=-59.}
$$

For the discriminant calculation, $f'(\alpha)=3\alpha^2+4\alpha$. In the [basis](../../../../basis.md) $1,\alpha,\alpha^2$, using $\alpha^3=-2\alpha^2-1$, multiplication by this element has [matrix](../../../../matrix.md)

$$
M=\begin{pmatrix}0&-3&2\\4&0&-3\\3&-2&4\end{pmatrix},\qquad\det M=59.
$$

Thus the given derivative-norm formula gives $D(1,\alpha,\alpha^2)=-59$. Since $\alpha$ satisfies a [monic polynomial](../../../../monic-polynomial.md) with [integer](../../../../integer-split.md) coefficients, $1,\alpha,\alpha^2$ are [algebraic integers](../../../../algebraic-integer.md); the fact that a [squarefree discriminant certifies an integral basis](../../../../squarefree-discriminant-certifies-an-integral-basis.md) proves

$$
\boxed{\mathcal O_K=\mathbb Z[\alpha],\qquad D_K=-59.}
$$

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the number theory course of the University of Oxford](../../../split.md)
5. [Number theory course of the University of Oxford](../../../../number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
