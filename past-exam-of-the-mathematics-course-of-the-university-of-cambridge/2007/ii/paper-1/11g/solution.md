<h1 id="11g/solution">Solution</h1>

↑ **Parent:** [11G](../11g.md)

For binary [linear codes](../../../../../linear-code.md) of length $n$, the [bar product of binary linear codes](../../../../../bar-product-of-binary-linear-codes.md) is $C_1|C_2=\{(u,u+v):u\in C_1,v\in C_2\}$. The parametrization is [injective](../../../../../injective-function.md) and linear, so its [dimension](../../../../../dimension-vector-space.md) is $k_1+k_2$. If $v=0$, a nonzero word has [Hamming weight](../../../../../hamming-weight.md) at least $2d_1$; if $v\ne0$, $\operatorname{wt}(u)+\operatorname{wt}(u+v)\ge\operatorname{wt}(v)\ge d_2$. Taking $(u,u)$ and $(0,v)$ of minimum weight shows

$$
\boxed{\dim(C_1|C_2)=k_1+k_2,\qquad d(C_1|C_2)=\min(2d_1,d_2).}
$$

For $a\in C_2^\perp,b\in C_1^\perp$, the inner product of $(u,u+v)$ and $(a,a+b)$ is $u\cdot b+v\cdot a+v\cdot b=0$, since $C_2\subseteq C_1$. The spaces have complementary [dimensions](../../../../../dimension-vector-space.md), proving $(C_1|C_2)^\perp=C_2^\perp|C_1^\perp$.

Define the [Reed-Muller code](../../../../../reed-muller-code.md) $\operatorname{RM}(d,r)$ by evaluating all multilinear [polynomials](../../../../../polynomial-split.md) of total degree at most $r$ at the $2^d$ points of $\mathbb F_2^d$. The squarefree monomials are independent functions, giving dimension $\sum_{j=0}^r\binom dj$. Splitting according to the last variable gives the [Reed-Muller bar-product recursion](../../../../../reed-muller-bar-product-recursion.md) $\operatorname{RM}(d,r)=\operatorname{RM}(d-1,r)|\operatorname{RM}(d-1,r-1)$, with the endpoint codes interpreted in the usual way. The distance recursion gives $2^{d-r}$.

To identify the [Dual of a Reed-Muller code](../../../../../dual-of-a-reed-muller-code.md), multiply a monomial of degree at most $r$ by one of degree at most $d-r-1$. The product omits some variable, so its sum over $\mathbb F_2^d$ is even and its binary inner product is zero. The binomial dimension identity then gives

$$
\boxed{\operatorname{RM}(d,r)^\perp=\operatorname{RM}(d,d-r-1)\quad(0\le r<d).}
$$

## ↑ Ancestors (10)

1. [11G](../11g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
