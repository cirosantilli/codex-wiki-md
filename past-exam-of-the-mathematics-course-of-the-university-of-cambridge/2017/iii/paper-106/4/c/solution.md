<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The prescribed-pole form of [Runge theorem](../../../../../../runge-s-theorem.md) is this: let $K\subset\mathbb C$ be compact, and let $E\subset\widehat{\mathbb C}\setminus K$ meet every [connected component](../../../../../../connected-component.md) of the complement in the [Riemann sphere](../../../../../../riemann-sphere.md). If $f$ is holomorphic on a neighbourhood of $K$, then for every $\epsilon>0$ there is a [rational function](../../../../../../rational-function.md) with all its poles in $E$ whose uniform distance from $f$ on $K$ is less than $\epsilon$. A polynomial is regarded as having its only possible pole at infinity. The empty compact set is trivial, so assume $K\ne\varnothing$.

First suppose $\infty\in E$. Let $A\subset C(K)$ be the [uniform rational approximation algebra with prescribed poles](../../../../../../uniform-rational-approximation-algebra-with-prescribed-poles.md), the uniform closure of [rational functions](../../../../../../rational-function.md) whose finite poles lie in $E$. It is a commutative unital [Banach algebra](../../../../../../banach-algebra-split.md), and contains $u(z)=z$. Set

$$
S=\{\lambda\in\mathbb C\setminus K:(u-\lambda1)^{-1}\in A\},
$$

where the inverse in this definition is the pointwise [continuous function](../../../../../../continuous-function.md) on $K$. The set $S$ is relatively open: if the inverse at $\lambda$ belongs to $A$, the [Neumann series](../../../../../../neumann-series.md) gives inverses at nearby points. It is relatively closed: when $\lambda_n\to\lambda\notin K$, the corresponding scalar functions converge uniformly on $K$, and $A$ is closed.

Each bounded complementary component meets $E$ in a finite point $a$, and $(u-a1)^{-1}$ is an allowed [rational function](../../../../../../rational-function.md). The unbounded component meets $S$ because for $|\lambda|>\|u\|$ the geometric series for $(u-\lambda1)^{-1}$ belongs to $A$. Being both open and closed in the complement, $S$ therefore contains every component, so it is the entire complement. Conversely, evaluation at any $z\in K$ prevents $u-z1$ from being invertible. Hence

$$
\boxed{\sigma_A(u)=K.}
$$

Apply the [holomorphic functional calculus](../../../../../../holomorphic-functional-calculus.md) in $A$ to $f$ near $K$. For every $z\in K$, the evaluation [character of an algebra](../../../../../../character-of-an-algebra.md) and the contour formula from (b) give $f(u)(z)=f(z)$. Thus $f|_K\in A$. By the definition of this uniform closure, the required rational approximations exist.

If $\infty\notin E$, choose a finite point $a\in E$ in the component containing infinity. The [Möbius transformation](../../../../../../mobius-transformation.md) $w=(z-a)^{-1}$ sends $K$ to a compact subset $K'$ of the plane and sends $E$ to a set $E'$ containing infinity. It preserves complementary components, so $E'$ meets every component of the complement of $K'$. The transformed function $F(w)=f(a+1/w)$ is holomorphic near $K'$, since $0\notin K'$. The case already proved approximates $F$ by [rational functions](../../../../../../rational-function.md) with poles in $E'$. Pulling them back gives rational approximations to $f$ on $K$ with poles only in $E$: a pole at infinity in the $w$-plane becomes a pole at $a$, and every other pole has its prescribed preimage. In particular the pullbacks do not acquire a pole at the original infinity, since $0\notin E'$.

This proves the full prescribed-pole theorem, including the case where a pole at infinity is forbidden. If $\mathbb C\setminus K$ is connected, take $E=\{\infty\}$ to obtain the [polynomial Runge theorem](../../../../../../polynomial-runge-theorem.md) as a corollary.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
