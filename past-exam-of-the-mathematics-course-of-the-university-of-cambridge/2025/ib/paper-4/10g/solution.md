<h1 id="10g/solution">Solution</h1>

↑ **Parent:** [10G](../10g.md)

A map $f:\mathbb R^n\to\mathbb R^m$ is [differentiable](../../../../../differentiable-function.md) at $x$ if there is a [linear map](../../../../../linear-map.md) $L$ such that

$$
f(x+h)=f(x)+Lh+o(\lVert h\rVert);
$$

then $Df|_x=L$. The [inverse function theorem](../../../../../inverse-function-theorem.md) says that if $f$ is continuously [differentiable](../../../../../differentiable-function.md) near $x$ and $Df|_x$ is invertible, then $f$ restricts to a $C^1$ diffeomorphism between neighborhoods of $x$ and $f(x)$.

Since $F(A)=A^TA$ is [polynomial](../../../../../polynomial-split.md),

$$
DF|_A(H)=H^TA+A^TH.
$$

Thus $\ker DF|_I=T$, the space of skew-symmetric [matrices](../../../../../matrix.md).

Define

$$
\Phi(A)=A^TA+A-A^T-I.
$$

Then $D\Phi|_I(H)=2H$, so the inverse [function](../../../../../function-split.md) theorem supplies open neighborhoods $I\in U$, $0\in V$ on which $\Phi:U\to V$ is a $C^1$ diffeomorphism. Its symmetric part is $A^TA-I$ and its skew part is $A-A^T$. Consequently

$$
\Phi(A)\in T\iff A^TA=I,
$$

and therefore $\Phi(U\cap\mathcal O)=V\cap T$.

For any $R\in\mathcal O$, left multiplication $A\mapsto R^TA$ is a homeomorphism preserving $\mathcal O$ and carrying $R$ to $I$. Transporting the preceding chart gives a neighborhood of $R$ in $\mathcal O$ homeomorphic to an open subset of $T$.

## ↑ Ancestors (10)

1. [10G](../10g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
