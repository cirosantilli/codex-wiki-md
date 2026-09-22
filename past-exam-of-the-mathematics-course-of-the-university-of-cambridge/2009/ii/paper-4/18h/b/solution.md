<h1 id="18h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A primitive tenth root $\xi$ has $\xi^5=-1$ and $\xi\ne-1$, so division of $X^5+1$ by $X+1$ gives

$$
\Phi_{10}(X)=X^4-X^3+X^2-X+1.
$$

It is irreducible over $\mathbb Q$: replacing $X$ by $-X$ gives $\Phi_5(X)$, and then replacing $X$ by $X+1$ gives $X^4+5X^3+10X^2+10X+5$. Any nontrivial monic integer factorization would reduce modulo five to factors that are powers of $X$, forcing both constant terms divisible by five and their product divisible by $25$, contrary to the constant term five. Rational factorization reduces to integer factorization by [Gauss lemma](../../../../../../gauss-s-lemma-riemannian-geometry.md): products of primitive integer [polynomials](../../../../../../polynomial-split.md) are primitive, since reduction modulo any prime preserves a nonzero product. Thus

$$
\boxed{\operatorname{min}_{\mathbb Q}(\xi)=X^4-X^3+X^2-X+1.}
$$

Let $t=\xi+\xi^{-1}$. Dividing $\Phi_{10}(\xi)=0$ by $\xi^2$ gives $t^2-t-1=0$. Hence $(2t-1)^2=5$, so $\boxed{\sqrt5\in\mathbb Q(\xi)}$. Either sign of this square root suffices; for $\xi=e^{\pi i/5}$ the positive one is $2t-1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [18H](../../18h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
