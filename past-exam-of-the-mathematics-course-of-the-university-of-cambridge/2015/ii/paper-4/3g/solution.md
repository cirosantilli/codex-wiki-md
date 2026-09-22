<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

Work over the [finite field](../../../../../finite-field.md) $\mathbb F_2$. Reduce [polynomials](../../../../../polynomial-split.md) modulo $X_i^2-X_i$, so their monomials are square-free. The binary [Reed-Muller code](../../../../../reed-muller-code.md) $\operatorname{RM}(r,m)$ consists of the evaluation vectors of [polynomials](../../../../../polynomial-split.md) of degree at most $r$ at all $2^m$ points of $\mathbb F_2^m$, in a fixed order. This is a [linear code](../../../../../linear-code.md) of length $2^m$ and dimension $\sum_{j=0}^r\binom mj$, for $0\leq r\leq m$. Square-free monomials give independent evaluation functions, as follows inductively by splitting according to the last variable.

The [minimum Hamming distance of a linear code](../../../../../minimum-hamming-distance-of-a-linear-code.md) equals its least nonzero [Hamming weight](../../../../../hamming-weight.md). The result is

$$
\boxed{d(\operatorname{RM}(r,m))=2^{m-r}\quad(0\leq r\leq m).}
$$

Here $r=0$ is the [repetition code](../../../../../repetition-code.md), while $r=m$ is the full binary vector space and has distance one. For the induction step, write $f(x,t)=u(x)+t v(x)$, where $\deg u\leq r$ and $\deg v\leq r-1$. Its evaluation vector is $(u,u+v)$, the [Reed-Muller bar-product recursion](../../../../../reed-muller-bar-product-recursion.md). If $v=0$, its nonzero [Hamming weight](../../../../../hamming-weight.md) is at least $2d(r,m-1)=2^{m-r}$, with the full-space endpoint treated as above. If $v\ne0$, every position where $v=1$ contributes exactly one to the sum of the two weights; hence the weight is at least $\operatorname{wt}(v)\geq2^{(m-1)-(r-1)}=2^{m-r}$. The monomial $X_1\cdots X_r$ is one exactly on $2^{m-r}$ points, attaining the bound. Degrees greater than $m$ give the same full code; the zero code at negative degree has no nonzero word whose weight could define a finite minimum.

## ↑ Ancestors (10)

1. [3G](../3g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
