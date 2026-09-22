# Polynomial Lax representation of the Nahm equations

↑ **Parent:** [Nahm equations](nahm-equations.md)

Put $P=A_1+iA_2$, $Q=A_1-iA_2$ and $R=A_3$, and define

$$
L(\lambda)=P+2R\lambda-Q\lambda^2,\qquad
M(\lambda)=-iR+iQ\lambda.
$$

Direct expansion gives $[L,M]=-i[P,R]+i[P,Q]\lambda+i[R,Q]\lambda^2$. The [Nahm equations](nahm-equations.md) imply $\dot P=-i[P,R]$, $2\dot R=i[P,Q]$ and $-\dot Q=i[R,Q]$, so $\dot L=[L,M]$. In any finite-dimensional [matrix](matrix.md) representation, cyclicity of the [matrix trace](matrix-trace.md) gives

$$
\frac d{dt}\operatorname{Tr}L^p
=p\operatorname{Tr}(L^{p-1}[L,M])=0\qquad(p=1,2,\ldots).
$$

Thus every coefficient of the degree-at-most-$2p$ [matrix trace](matrix-trace.md) polynomial is conserved. At projective infinity the polynomial is interpreted as a section of $\mathcal O(2p)$, not a globally [holomorphic](complex-differentiability-at-a-point.md) scalar function on the [complex projective line](complex-projective-line.md).

## ↑ Ancestors (10)

1. [Nahm equations](nahm-equations.md)
2. [Anti-self-dual Yang-Mills equations in temporal gauge](anti-self-dual-yang-mills-equations-in-temporal-gauge.md)
3. [Anti-self-dual Yang-Mills equations](anti-self-dual-yang-mills-equations.md)
4. [Yang-Mills instanton](yang-mills-instanton.md)
5. [Gauge-theory soliton](gauge-theory-soliton.md)
6. [Classical field-theory soliton](classical-field-theory-soliton-split.md)
7. [Quantum field theory](quantum-field-theory-split.md)
8. [Branches of physics](branches-of-physics.md)
9. [Physics](physics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-56/3/solution.md)
