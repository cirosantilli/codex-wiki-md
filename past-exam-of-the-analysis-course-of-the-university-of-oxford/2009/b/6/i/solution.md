<h1 id="b/6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Hilbert projection theorem](../../../../../hilbert-projection-theorem.md) states that every vector $x$ has a unique decomposition $x=m+n$ relative to a closed [linear subspace](../../../../../vector-subspace.md) $M$, with $m\in M$ and $n\in M^\perp$. The vector $m$ is the unique nearest point in $M$.

The [Riesz representation theorem](../../../../../riesz-representation-theorem.md) states that every bounded complex-[linear functional](../../../../../linear-functional.md) $F$ on a [Hilbert space](../../../../../hilbert-space-split.md) has a unique representation $F(x)=\langle x,y\rangle$, with $\|F\|=\|y\|$, using the convention of linearity in the first argument. If $F=0$, use $y=0$. Otherwise $M=\ker F$ is closed. Project a vector outside $M$ to obtain $z\in M^\perp$ with $F(z)\ne0$, and rescale it so $F(z)=1$. Then $x-F(x)z\in M$, so

$$
\langle x,z\rangle=F(x)\|z\|^2,\qquad y=z/\|z\|^2.
$$

This gives the representation. Uniqueness follows because a vector orthogonal to every $x$ is zero. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $\|F\|\leq\|y\|$, and evaluation at $y/\|y\|$ gives equality when $y\ne0$.

For the adjoint, fix $v$. The functional $u\mapsto\langle Tu,v\rangle$ is bounded with [norm](../../../../../norm.md) at most $\|T\|\|v\|$. By the [Riesz representation theorem](../../../../../riesz-representation-theorem.md), there is a unique vector $T^*v$ satisfying

$$
\boxed{\langle u,T^*v\rangle=\langle Tu,v\rangle\quad(u\in V).}
$$

For scalars $a,b$, conjugate-linearity in the second argument shows that $T^*(av+bw)=aT^*v+bT^*w$, by uniqueness of the representing vector. The same [norm](../../../../../norm.md) estimate gives $\|T^*v\|\leq\|T\|\|v\|$. Thus $T^*$ is a unique [bounded linear operator](../../../../../continuous-linear-operator.md), the [adjoint operator](../../../../../adjoint-operator.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the analysis course of the University of Oxford](../../../../split.md)
6. [Analysis course of the University of Oxford](../../../../../analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
