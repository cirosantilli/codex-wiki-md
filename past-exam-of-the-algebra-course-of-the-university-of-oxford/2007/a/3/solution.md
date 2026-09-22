<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Each $M_i$ is an [ideal](../../../../ideal.md) because the [algebra](../../../../algebra-split.md) is commutative. For $m\in M_i$, the product $me_j$ belongs both to $M_i$ and $M_j$, so is zero when $j\ne i$. Multiplying $1=\sum_je_j$ by $m$ therefore gives $m=me_i$. In particular $e_i^2=e_i$, different $e_i$ have zero product, and

$$
\boxed{M_i=Ae_i,\qquad e_i^2=e_i,\qquad e_ie_j=0\ (i\ne j).}
$$

For any [idempotent](../../../../idempotent.md) $e$, the set $Ae$ is closed under multiplication and $e$ acts as its identity. With $f=1-e$ the map $a\mapsto(ae,af)$ is an [algebra](../../../../algebra-split.md) isomorphism $A\to Ae\times Af$: multiplication is componentwise because $ef=0$, and its inverse sends $(u,v)$ to $u+v$.

The $A$-[submodules](../../../../submodule.md) of $Ae$ are exactly its [ideals](../../../../ideal.md) as a unital [algebra](../../../../algebra-split.md), since acting by $a$ on $Ae$ is the same as acting by $ae$. A nonzero commutative unital [algebra](../../../../algebra-split.md) is a [simple module](../../../../irreducible-module.md) over itself exactly when every nonzero principal [ideal](../../../../ideal.md) is the whole [algebra](../../../../algebra-split.md), which is equivalent to every nonzero element having an inverse. Thus **a nonzero component $Ae$ is simple exactly when it is a [field](../../../../field.md)**. If $e=0$, both properties fail under the nonzero-[field](../../../../field.md) convention.

A semisimple regular [module](../../../../module-mathematics.md) is a finite [direct sum](../../../../direct-sum.md) of simple [ideals](../../../../ideal.md). Applying the preceding decomposition gives a finite direct product of [fields](../../../../field.md). Conversely the coordinate [ideals](../../../../ideal.md) of a finite product of [fields](../../../../field.md) are [simple modules](../../../../irreducible-module.md), so its regular [module](../../../../module-mathematics.md) is semisimple. The [fields](../../../../field.md) are finite extensions of $K$, because $A$ has finite $K$-[dimension](../../../../dimension-vector-space.md).

For a generator $g$ of the [cyclic group](../../../../cyclic-group.md) of order three, evaluation $X\mapsto g$ gives a surjection $\mathbb Q[X]\to\mathbb QG$ with [kernel](../../../../kernel-of-a-linear-map-split.md) $(X^3-1)$, by division and independence of $1,g,g^2$. The factors $X-1$ and $X^2+X+1$ are coprime, and the quadratic is irreducible over $\mathbb Q$. The [Chinese remainder theorem](../../../../chinese-remainder-theorem.md) yields

$$
\boxed{\mathbb QG\cong\frac{\mathbb Q[X]}{(X^3-1)}\cong\mathbb Q\times\mathbb Q(\sqrt{-3}).}
$$

The explicit map sends $g$ to $(1,\zeta_3)$, where $\zeta_3=(-1+\sqrt{-3})/2$.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the algebra course of the University of Oxford](../../../split.md)
5. [Algebra course of the University of Oxford](../../../../algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
