<h1 id="11g/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Factor $X^3+X=X(X-i)(X+i)$. These factors generate pairwise comaximal [ideals](../../../../../../ideal.md), so the [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) gives

$$
\Phi([p])=(p(0),p(i),p(-i)).
$$

The three copies of $\mathbb C$ have different [module](../../../../../../module-mathematics.md) structures: $X$ acts by $0,i,-i$, respectively. Thus $q(X)$ acts on $(a,b,c)$ as $(q(0)a,q(i)b,q(-i)c)$, making $\Phi$ a [module homomorphism](../../../../../../module-homomorphism.md).

The inverse, obtained by [Lagrange interpolation](../../../../../../lagrange-polynomial.md), is

$$
\boxed{\Phi^{-1}(a,b,c)=\left[a(1+X^2)-\frac b2(X^2+iX)-\frac c2(X^2-iX)\right].}
$$

Evaluating at $0,i,-i$ recovers $(a,b,c)$. Conversely, a polynomial whose three evaluations vanish is divisible by $X(X-i)(X+i)$, so these maps are mutual inverses on the [quotient module](../../../../../../quotient-module.md). Three copies with identical trivial $X$-action would not give the required isomorphism.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [11G](../../11g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
