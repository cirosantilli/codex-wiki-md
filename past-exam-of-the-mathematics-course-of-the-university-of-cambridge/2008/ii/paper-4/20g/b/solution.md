<h1 id="20g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [polynomial](../../../../../../polynomial-split.md) $T^4-2$ is irreducible by [Eisenstein criterion](../../../../../../eisenstein-criterion.md) at two, so $1,\alpha,\alpha^2,\alpha^3$ is a rational basis and each of these elements is integral. The nontrivial automorphism of $K/k$ sends $\alpha$ to $-\alpha$. For an [algebraic integer](../../../../../../algebraic-integer.md) $\theta$, its [relative trace](../../../../../../relative-trace.md) and the trace of the [algebraic integer](../../../../../../algebraic-integer.md) $\alpha\theta$ are

$$
\operatorname{Tr}_{K/k}\theta=2a+2c\sqrt2,\qquad
\operatorname{Tr}_{K/k}(\alpha\theta)=4d+2b\sqrt2.
$$

Both are in $\mathcal O_k$, proving $2a,2b,2c,4d\in\mathbb Z$. Multiplying $\theta$ by its conjugate gives the [field norm](../../../../../../field-norm.md)

$$
\operatorname N_{K/k}\theta
=(a+c\sqrt2)^2-\sqrt2(b+d\sqrt2)^2
=(a^2+2c^2-4bd)+(2ac-b^2-2d^2)\sqrt2.
$$

Again this is in $\mathcal O_k$, so both displayed coefficients are integers.

To finish the denominator argument, put $A=2a$, $B=2b$, $C=2c$, $D=4d$, all integers. The two norm coefficients imply

$$
A^2+2C^2-2BD\equiv0\pmod4,\qquad
4AC-2B^2-D^2\equiv0\pmod8.
$$

The second congruence modulo two first gives $D$ even. Modulo four it then gives $B$ even. Therefore $2BD$ vanishes modulo four, and the first congruence reads $A^2+2C^2\equiv0\pmod4$. The possible squares modulo four force $A$ even and then $C$ even. Returning to the second congruence now gives $D^2\equiv0\pmod8$, so $D$ is divisible by four. Thus $a,b,c,d$ are all integers.

Conversely, every integer linear combination of these powers is integral. We have proved the [integral basis of the fourth-root-of-two field](../../../../../../integral-basis-of-the-fourth-root-of-two-field.md):

$$
\boxed{\mathcal O_K=\mathbb Z[\alpha],\qquad1,\alpha,\alpha^2,\alpha^3\text{ is an integral basis}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [20G](../../20g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
