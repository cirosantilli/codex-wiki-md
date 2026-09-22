<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First recall why the two-variable [Bézout's identity](../../../../../../bezout-s-identity.md) follows from the [Euclidean algorithm](../../../../../../euclidean-algorithm.md). The initial values $a,b$ are [integer linear combinations](../../../../../../integer-linear-combination.md) of $a,b$. At every subsequent step, $r_{j+1}=r_{j-1}-q_jr_j$ is again an [integer linear combination](../../../../../../integer-linear-combination.md) of $a,b$. Therefore the last nonzero [remainder](../../../../../../remainder.md), which is their [greatest common divisor](../../../../../../greatest-common-divisor.md), has that form.

Put $e=\gcd(a,b)$. The preceding argument supplies [integers](../../../../../../integer-split.md) $u,v$ with $e=au+bv$. Applying the same argument to $e,c$ gives [integers](../../../../../../integer-split.md) $p,q$ such that

$$
\gcd(e,c)=ep+cq.
$$

An [integer](../../../../../../integer-split.md) divides $a,b,c$ exactly when it divides $e,c$: if it divides $a,b$, it divides $e=au+bv$, while $e$ itself divides both $a,b$. Hence $\gcd(e,c)=\gcd(a,b,c)=d$. Substituting the expression for $e$ proves

$$
d=(au+bv)p+cq=a(up)+b(vp)+cq.
$$

Thus

$$
\boxed{x=up,\qquad y=vp,\qquad z=q}
$$

are [integers](../../../../../../integer-split.md) satisfying $ax+by+cz=d$. This also explains how to construct the coefficients using two applications of the [Euclidean algorithm](../../../../../../euclidean-algorithm.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
