<h1 id="12i/solution">Solution</h1>

↑ **Parent:** [12I](../12i.md)

The [primitive recursive functions](../../../../../primitive-recursive-function.md) are the smallest class containing zero, successor, and projections and closed under composition and primitive recursion. Addition is defined by

$$
P(m,0)=m,
\qquad P(m,n+1)=S(P(m,n)),
$$

and multiplication by

$$
T(m,0)=0,
\qquad T(m,n+1)=P(T(m,n),m).
$$

Thus both are primitive recursive directly from the definition. Inductively,

$$
T_{k+1}(n_1,\ldots,n_{k+1})
=T(T_k(n_1,\ldots,n_k),n_{k+1})
$$

is primitive recursive. For fixed $a$,

$$
E_a(0)=1,
\qquad E_a(n+1)=T(a,E_a(n)),
$$

so $E_a(n)=a^n$ is primitive recursive.

Encode $(x_0,\ldots,x_{k-1})$ by $2^{x_0}3^{x_1}\cdots p_k^{x_{k-1}}$. The exponent functions $M_{p_i}$ decode the coordinates. Therefore

$$
\overline F(N)=
\prod_{i=0}^{k-1}p_{i+1}^{
 f_i(M_2(N),M_3(N),\ldots,M_{p_k}(N))}
$$

is a primitive recursive one-number encoding of $F$; the finite product is built from the primitive recursive multiplication and exponentiation just established.

The Fibonacci function is primitive recursive. Encode the pair $(B(n),B(n+1))$ by

$$
C(n)=2^{B(n)}3^{B(n+1)}.
$$

Starting with $C(0)=3$, primitive recursion using

$$
C(n+1)=2^{M_3(C(n))}
3^{M_2(C(n))+M_3(C(n))}
$$

constructs $C$, and $B(n)=M_2(C(n))$.

There is no universal exponential bound of the stated form. The primitive recursive function

$$
f(n)=2^{n^2}
$$

exceeds $R^n$ for every fixed $R>0$ once $n$ is sufficiently large.

## ↑ Ancestors (10)

1. [12I](../12i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
