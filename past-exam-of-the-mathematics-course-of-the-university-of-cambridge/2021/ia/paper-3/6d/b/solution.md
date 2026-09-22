<h1 id="6d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The orbit of $(1,\ldots,k)$ consists precisely of the ordered $k$-tuples of distinct elements of $\{1,\ldots,n\}$:

$$
\operatorname{Orb}(x)
=\{(x_1,\ldots,x_k):x_i\ne x_j\text{ for }i\ne j\}.
$$

It has size

$$
n(n-1)\cdots(n-k+1)=\frac{n!}{(n-k)!}.
$$

The stabilizer consists of permutations fixing $1,\ldots,k$ pointwise, while freely permuting the remaining letters:

$$
\operatorname{Stab}(x)\cong S_{n-k},
\qquad
|\operatorname{Stab}(x)|=(n-k)!.
$$

Thus

$$
|\operatorname{Orb}(x)|\,|\operatorname{Stab}(x)|
=\frac{n!}{(n-k)!}(n-k)!=n!=|S_n|,
$$

verifying orbit-stabilizer.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6D](../../6d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
