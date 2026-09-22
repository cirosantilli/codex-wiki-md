<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) assumes that $H$ is a real [Hilbert space](../../../../../../hilbert-space-split.md) and $B:H\times H\to\mathbb R$ is a [bounded bilinear form](../../../../../../bounded-bilinear-form.md) and a [coercive bilinear form](../../../../../../coercive-bilinear-form.md): there are $M,\alpha>0$ such that

$$
|B[u,v]|\leq M\|u\|_H\|v\|_H,\qquad
B[u,u]\geq\alpha\|u\|_H^2.
$$

Then for every [continuous linear functional](../../../../../../continuous-linear-functional.md) $\ell\in H'$ there is a unique $u\in H$ satisfying

$$
\boxed{B[u,v]=\ell(v)\quad(v\in H),\qquad
\|u\|_H\leq\alpha^{-1}\|\ell\|_{H'}.}
$$

Symmetry of $B$ is not required.

For the proof, the [Riesz representation theorem](../../../../../../riesz-representation-theorem.md) provides a [bounded linear operator](../../../../../../continuous-linear-operator.md) $T:H\to H$ and $g\in H$ with $B[u,v]=(Tu,v)_H$ and $\ell(v)=(g,v)_H$. Coercivity and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) imply

$$
\alpha\|u\|_H^2\leq(Tu,u)_H\leq\|Tu\|_H\|u\|_H,
\qquad\|Tu\|_H\geq\alpha\|u\|_H.
$$

Thus $T$ is injective and its range is closed: if $Tu_j$ converges, the displayed inequality makes $u_j$ a [Cauchy sequence](../../../../../../cauchy-sequence.md); [completeness](../../../../../../completeness.md) gives $u_j\to u$ and $Tu_j\to Tu$. If $w$ lies in the [orthogonal complement](../../../../../../orthogonal-complement.md) of the range, then $B[v,w]=0$ for all $v$. Taking $v=w$ gives $\alpha\|w\|^2\leq B[w,w]=0$, so $w=0$. A closed subspace with zero [orthogonal complement](../../../../../../orthogonal-complement.md) is all of $H$, hence $T$ is surjective. The unique solution is $T^{-1}g$, and the same inequality gives the asserted norm bound.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
