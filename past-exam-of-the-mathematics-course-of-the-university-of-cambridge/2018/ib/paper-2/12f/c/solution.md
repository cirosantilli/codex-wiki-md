<h1 id="12f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $P_n$ be the [finite-dimensional vector space](../../../../../../finite-dimensional-vector-space.md) of real polynomials of degree at most $n$. For fixed $a>0$,

$$
N(p)=\sup_{x\in[0,a]}|p(x)|
$$

is a [norm](../../../../../../norm.md): if it vanishes, the polynomial vanishes on an interval and hence is the zero polynomial. Also

$$
M(p)=N(p)+\sup_{x\in[0,1]}|p'(x)|
$$

is a norm on $P_n$. By [finite-dimensional equivalence of norms](../../../../../../finite-dimensional-equivalence-of-norms.md), there is $C>0$, depending only on $n$ and $a$, such that $M(p)\leq C N(p)$. Therefore

$$
\sup_{x\in[0,1]}|p'(x)|\leq C\sup_{x\in[0,a]}|p(x)|.
$$

The [extreme value theorem](../../../../../../extreme-value-theorem.md) supplies $y\in[0,a]$ at which the last supremum is attained, and hence

$$
\boxed{\sup_{x\in[0,1]}|p'(x)|\leq C|p(y)|.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
