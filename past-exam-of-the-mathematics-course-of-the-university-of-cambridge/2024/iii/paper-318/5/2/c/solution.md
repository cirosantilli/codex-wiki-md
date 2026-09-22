<h1 id="5/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For any admissible $f$, part (a) rewrites the constraints as

$$
(M_i,f^{(k)})=k!\gamma_i=(M_i,s),
\qquad i=1,\ldots,n.
$$

Hence $f^{(k)}-s$ is orthogonal to every $M_i$ and therefore to their span, which contains $s$. The [Pythagorean theorem in an inner-product space](../../../../../../../pythagorean-theorem-in-an-inner-product-space.md) gives

$$
\|f^{(k)}\|_2^2
=\|s\|_2^2+\|f^{(k)}-s\|_2^2
\geq\|s\|_2^2.
$$

Choose any $k$-fold antiderivative $\sigma$ of $s$. The identity from part (a) and $(M_i,s)=k!\gamma_i$ show that $\sigma$ satisfies all prescribed divided differences, and equality holds in the norm bound. Therefore

$$
\boxed{\sigma^{(k)}=s}
$$

characterizes the minimizers. They are unique up to addition of an arbitrary polynomial in $\mathcal P_{k-1}$, which changes neither the order-$k$ divided differences nor the $k$th derivative.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [5](../../../5.md)
4. [Paper 318](../../../../paper-318-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
