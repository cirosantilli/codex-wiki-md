<h1 id="11h/solution">Solution</h1>

↑ **Parent:** [11H](../11h.md)

For length-$n$ binary [linear codes](../../../../../linear-code.md) $C_2\subseteq C_1$, their [bar product of binary linear codes](../../../../../bar-product-of-binary-linear-codes.md) is

$$
C_1|C_2=\{(u,u+v):u\in C_1, v\in C_2\}.
$$

The map $(u,v)\mapsto(u,u+v)$ is injective and linear, so

$$
\dim(C_1|C_2)=\dim C_1+\dim C_2.
$$

If $d_i$ is the minimum distance of $C_i$, then

$$
\operatorname{wt}(u)+\operatorname{wt}(u+v)
\geq\operatorname{wt}(v).
$$

For $v\ne0$ this is at least $d_2$; for $v=0$ a nonzero word has weight at least $2d_1$. Words $(0,v)$ and $(u,u)$ attain these bounds, proving

$$
\boxed{\ d(C_1|C_2)=\min(d_2,2d_1)\ }.
$$

A [parity-check matrix](../../../../../parity-check-matrix.md) $P$ for a code $C$ is a matrix satisfying $C=\ker P$. A pair $(x,y)$ belongs to $C_1|C_2$ exactly when

$$
x\in C_1,\qquad x+y\in C_2.
$$

Thus a parity-check matrix is

$$
\boxed{\begin{pmatrix}
P_1&0\\
P_2&P_2
\end{pmatrix}}.
$$

This is the [parity-check matrix of a bar product](../../../../../parity-check-matrix-of-a-bar-product.md).

The [Reed-Muller code](../../../../../reed-muller-code.md) $\operatorname{RM}(d,r)$ is the length-$2^d$ binary code obtained by evaluating every square-free polynomial in $d$ Boolean variables of degree at most $r$ on all points of $\mathbb F_2^d$. Equivalently,

$$
\operatorname{RM}(d,r)
=\operatorname{RM}(d-1,r)\mid\operatorname{RM}(d-1,r-1).
$$

The square-free monomials form a basis, so

$$
\boxed{\ \dim\operatorname{RM}(d,r)=\sum_{j=0}^r\binom dj\ }.
$$

A word in $\operatorname{RM}(d,1)$ evaluates an affine function $a_0+a\cdot x$. The two constant functions have weights $0$ and $2^d$. Every nonconstant affine function takes each value equally often, so all other codewords have weight $2^{d-1}$.

A monomial of degree $j$ has weight $2^{d-j}$. Hence every generator, and therefore every codeword, has even weight when $r<d$. For $r=d$, the monomial $x_1\cdots x_d$ has weight one. **All words have even weight exactly for $0\leq r\leq d-1$.**

## ↑ Ancestors (10)

1. [11H](../11h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
