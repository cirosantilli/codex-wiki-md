<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

[Lagrange theorem for polynomial congruences](../../../../../lagrange-theorem-for-polynomial-congruences.md) says that a nonzero [polynomial](../../../../../polynomial-split.md) of [degree](../../../../../degree-of-a-polynomial.md) $d$ over the [finite field](../../../../../finite-field.md) $\mathbb F_p$ has at most $d$ roots. To prove it, use [mathematical induction](../../../../../mathematical-induction.md) on $d$. A constant nonzero polynomial has no roots. If $f(a)=0$, [polynomial division](../../../../../polynomial-division.md) in the field $\mathbb F_p$ gives $f(X)=(X-a)q(X)$ with $\deg q=d-1$. Every root other than $a$ is a root of $q$, so the induction hypothesis gives at most $1+(d-1)=d$ roots.

Every nonzero [residue class](../../../../../residue-class.md) modulo $p$ has a unique [multiplicative inverse](../../../../../modular-multiplicative-inverse.md). In the product $(p-1)!$, pair each class with its inverse. The unpaired classes satisfy $x=x^{-1}$, hence $x^2-1=0$. By the theorem these are exactly $1$ and $-1$, and therefore

$$
(p-1)!\equiv1\cdot(-1)\equiv-1\pmod p.
$$

This is [Wilson theorem](../../../../../wilson-s-theorem.md).

Now write $p-1=kq$. By [Fermat's little theorem](../../../../../fermat-little-theorem.md), every nonzero class is a root of

$$
X^{p-1}-1=(X^k-1)(1+X^k+\cdots+X^{(q-1)k}).
$$

The second factor has degree $p-1-k$ and hence at most $p-1-k$ roots. Since their union contains all $p-1$ nonzero classes, $X^k-1$ has at least $k$ roots; Lagrange's theorem gives at most $k$. Thus $x^k\equiv1\pmod p$ has exactly $k$ solutions.

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
