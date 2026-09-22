<h1 id="b/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

A [Unitary element of a C-star algebra](../../../../unitary-element-of-a-c-star-algebra.md) satisfies $u^*u=uu^*=1$. A [projection in a C-star algebra](../../../../projection-in-a-c-star-algebra.md) satisfies $p=p^*=p^2$.

If $q=u^*u$ is a [projection in a C-star algebra](../../../../projection-in-a-c-star-algebra.md), the [C-star identity](../../../../c-star-identity.md) gives $\|u(1-q)\|^2=\|(1-q)q(1-q)\|=0$. Hence $u=uq=uu^*u$. Conversely $uu^*u=u$ implies $(u^*u)^2=u^*u$, and $u^*u$ is a [Hermitian C-star element](../../../../hermitian-element-of-a-c-star-algebra.md), so it is a [projection in a C-star algebra](../../../../projection-in-a-c-star-algebra.md). Taking adjoints of the triple-product equality gives the corresponding equality for $u^*$, proving

$$
\boxed{u\text{ partial isometry}\iff uu^*u=u\iff u^*\text{ partial isometry}.}
$$

For nonzero $u$, let $p=uu^*$ and $q=u^*u$. These are projections, $u=pu=uq$, and $\|u\|=1$. The rectangular corner $pAq$ is closed because it is the range of the bounded idempotent map $a\mapsto paq$.

Define $\Theta:pAq\to qAq$ by $\Theta(a)=u^*a$. It lands in the corner, and its inverse is $b\mapsto ub$. The identities $uu^*a=pa=a$ and $u^*ub=qb=b$ verify both compositions. Both maps are contractive because $\|u\|=\|u^*\|=1$, so $\Theta$ is an [isometry](../../../../isometry.md). For the proposed multiplication and [involution](../../../../involution.md),

$$
\Theta(au^*b)=\Theta(a)\Theta(b),\qquad\Theta(ua^*u)=q a^*u=a^*u=\Theta(a)^*.
$$

Thus the operations correspond exactly to the ordinary operations in the closed [C-star algebra](../../../../c-star-algebra.md) $qAq$. This proves associativity, [closure](../../../../closure-topology.md), all [involution](../../../../involution.md) identities and the C\*-[norm](../../../../norm.md) identity at once. Moreover $\Theta(u)=q$, so **the unit of $A_u$ is $u$**. If $u$ is unitary, $p=q=1$, and the map $a\mapsto u^*a$ is an onto isometric \*-isomorphism from $A_u$ to $A$.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../split.md)
5. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
