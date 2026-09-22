<h1 id="2f/solution">Solution</h1>

↑ **Parent:** [2F](../2f.md)

Write $\tau=(1+\sqrt{-3})/2$. The parity condition gives $R=\mathbb Z[\tau]$, since $(a+b\sqrt{-3})/2=(a-b)/2+b\tau$. For any such element,

$$
N(z)=z\overline z=\frac{a^2+3b^2}{4}\ge0.
$$

If $a,b$ are even the numerator is divisible by four; if they are odd it is congruent to $1+3=0$ modulo four. Therefore **$N(z)$ is a nonnegative integer**. It is zero only at zero, and the [Eisenstein-integer norm](../../../../../eisenstein-integer-norm.md) is multiplicative because [complex conjugation](../../../../../complex-conjugation.md) respects multiplication.

If $z$ is a unit, $N(z)N(z^{-1})=1$, so $N(z)=1$. Conversely $N(z)=1$ makes $\overline z$ its inverse in $R$. The equation $a^2+3b^2=4$ permits exactly $(a,b)=(\pm2,0)$ or $(\pm1,\pm1)$. Hence

$$
\boxed{R^\times=\{\pm1,\pm\tau,\pm\tau^2\},\qquad |R^\times|=6.}
$$

Indeed $\tau^2=\tau-1$ and $\tau^3=-1$, so this [unit group](../../../../../unit-group.md) is cyclic of order six.

For the prime-ideal assertion, $\tau^2-\tau+1=0$ and the polynomial $t^2-t+1$ has distinct roots $3,5$ modulo seven. Consequently evaluation at either root defines a surjective ring map $R\to\mathbb F_7$. Its kernels

$$
\mathfrak p=(7,\tau-3),\qquad\mathfrak q=(7,\tau-5)
$$

are distinct [maximal ideals](../../../../../maximal-ideal.md), hence [prime ideals](../../../../../prime-ideal.md). If $A+B\tau$ belongs to both, then $A+3B\equiv A+5B\equiv0\pmod7$. Subtraction gives $2B\equiv0$, so both $A$ and $B$ are divisible by seven. The converse inclusion is immediate, proving

$$
\boxed{7R=\mathfrak p\cap\mathfrak q.}
$$

Equivalently, the two distinct factors of the reduced polynomial give the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) decomposition $R/7R\cong\mathbb F_7\times\mathbb F_7$. This proof does not require the permitted unique-factorization assumption.

## ↑ Ancestors (10)

1. [2F](../2f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
