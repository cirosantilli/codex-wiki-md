<h1 id="18h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The pair $Z_n=(X_n,Y_n)$ is an irreducible positive recurrent [product Markov chain](../../../../../../product-markov-chain.md) with stationary distribution

$$
\Pi_{ij}=\pi_i\pi_j.
$$

The [stationary cycle occupation formula](../../../../../../stationary-cycle-occupation-formula.md) says that, during one return cycle to a state $z$, the expected number of visits to a set $A$ is $\Pi(A)/\Pi(z)$. Take

$$
z=(0,0),
\qquad A=\{(i,1):i\geq0\}.
$$

Then

$$
\Pi(A)=\pi_1=\frac14,
\qquad
\Pi(0,0)=\pi_0^2=\frac14.
$$

The initial and terminal states both have $Y=0$, so either convention for including the endpoints gives the same count. Thus

$$
\boxed{\mathbb E\!\left[\#\{0\leq n\leq T:Y_n=1\}\right]=1}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18H](../../18h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
