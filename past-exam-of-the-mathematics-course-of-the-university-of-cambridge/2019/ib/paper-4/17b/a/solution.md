<h1 id="17b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $D=d/dx$. Repeated [integration by parts](../../../../../../integration-by-parts.md) gives the [formal adjoint](../../../../../../formal-adjoint.md) rules

$$
D^*= -D,
\qquad
(pD^2)^*=D^2p=pD^2+2p'D+p'',
\qquad
(qD)^*=-Dq=-qD-q'.
$$

Therefore

$$
L^*=D^4+pD^2+(2p'-q)D+(p''-q'+r).
$$

Equality of the coefficients of $D$ in $L$ and $L^*$ requires

$$
q=2p'-q,
$$

so $q=p'$. This also makes the zeroth-order coefficients equal because $p''-q'=0$. Hence, under boundary conditions that remove the boundary terms,

$$
\boxed{L\text{ is self-adjoint}\iff q=p'}.
$$

This is the [self-adjoint fourth-order scalar differential operator](../../../../../../self-adjoint-fourth-order-scalar-differential-operator.md) $D^4+pD^2+p'D+r$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17B](../../17b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
