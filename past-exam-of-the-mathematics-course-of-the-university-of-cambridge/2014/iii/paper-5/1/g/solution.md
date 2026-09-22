<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The real [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) applies to a [Hilbert space](../../../../../../hilbert-space-split.md) $H$ and a [bounded bilinear form](../../../../../../bounded-bilinear-form.md) $a$ satisfying

$$
|a(u,v)|\leq M\|u\|\|v\|,\qquad a(v,v)\geq\alpha\|v\|^2\quad(\alpha>0).
$$

For every bounded [linear functional](../../../../../../linear-functional.md) $L$ there is a unique $u\in H$ with

$$
\boxed{a(u,v)=L(v)\quad(v\in H),\qquad\|u\|\leq\alpha^{-1}\|L\|.}
$$

Symmetry of the [bilinear form](../../../../../../bilinear-form.md) is not required.

By the [Riesz representation theorem](../../../../../../riesz-representation-theorem.md), write $a(u,v)=\langle Au,v\rangle$ and $L(v)=\langle g,v\rangle$. The operator $A$ is linear and bounded, with $\|A\|\leq M$. The [coercive bilinear form](../../../../../../coercive-bilinear-form.md) bound and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) imply

$$
\alpha\|u\|^2\leq\langle Au,u\rangle\leq\|Au\|\|u\|,
\qquad\|Au\|\geq\alpha\|u\|.
$$

Hence $A$ is injective. Its range is closed: if $Au_n$ converges, this last inequality applied to differences makes $u_n$ a [Cauchy sequence](../../../../../../cauchy-sequence.md), and its limit maps to the proposed range limit. If $w$ is in the [orthogonal complement](../../../../../../orthogonal-complement.md) of the range, then $a(u,w)=0$ for all $u$; taking $u=w$ and using coercivity gives $w=0$. The range is thus dense as well as closed, so it is all of $H$. Solve $Au=g$ uniquely; the displayed lower bound gives the asserted estimate.

For complex [Hilbert spaces](../../../../../../hilbert-space-split.md) the same proof works for a bounded [sesquilinear form](../../../../../../sesquilinear-form.md), linear in the first argument, with $\operatorname{Re}a(v,v)\geq\alpha\|v\|^2$. In the convention $a(u,v)=L(v)$, $L$ must then be a bounded conjugate-linear functional represented as $\langle g,v\rangle$.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [1](../../1.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
