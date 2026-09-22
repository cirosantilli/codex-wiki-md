<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [finite representation type of a quiver](../../../../../finite-representation-type-of-a-quiver.md) condition means there are only finitely many isomorphism classes of indecomposable finite-dimensional $kQ$-modules. Equivalently, every finite-dimensional [module](../../../../../module-mathematics.md) is a [direct sum](../../../../../direct-sum.md) of members of a finite list of indecomposables.

For the $E_6$ case, we give the reflection argument underlying the [Gabriel theorem](../../../../../gabriel-s-theorem.md), rather than using its conclusion as the proof. Since the underlying graph is a tree, every orientation is acyclic. At a sink $i$, write

$$
h:\bigoplus_{j\to i}V_j\longrightarrow V_i
$$

for the sum of the incoming arrow maps. If an indecomposable $V$ is not the simple $S_i$, then $h$ is surjective: a nonzero complementary subspace to its image at the sink would be a [direct summand](../../../../../direct-summand.md) supported only at $i$. The [Bernstein–Gelfand–Ponomarev reflection functor](../../../../../bernstein-gelfand-ponomarev-reflection-functor.md) reverses the arrows and replaces $V_i$ by $\ker h$, with reversed maps the component projections. The source reflection replaces that [kernel](../../../../../kernel-of-a-linear-map.md) by the [cokernel](../../../../../cokernel.md) of its inclusion into $\bigoplus V_j$, recovering $V_i$. The inclusion is injective, so the reflected representation has no [direct summand](../../../../../direct-summand.md) $S_i$ at the new source. If it decomposed, applying the inverse would decompose $V$. Thus reflection preserves indecomposability except that it annihilates $S_i$.

On a [dimension vector of a quiver representation](../../../../../dimension-vector-of-a-quiver-representation.md), it acts by the integral simple reflection

$$
(s_i d)_i=-d_i+\sum_{j\sim i}d_j,\qquad (s_i d)_j=d_j\quad(j\ne i).
$$

Let $B=2I-\operatorname{Adj}(E_6)$. These reflections preserve the [positive-definite quadratic form](../../../../../positive-definite-quadratic-form.md) $d^{\mathsf T}Bd$. Positivity can be checked without a classification theorem: label the graph by the chain $1-2-3-4-5$ and attach vertex $6$ to $3$. The leading principal minors are $2,3,4,5,6,3$, all positive.

Choose a topological ordering so arrows point from smaller to larger indices. Reflect successively at sinks $6,5,\ldots,1$. This restores the orientation after one full cycle. The transformation of dimension vectors is the [Coxeter element](../../../../../coxeter-element.md) $C=s_1s_2\cdots s_6$. If $U$ has diagonal entries one and entry $-1$ above the diagonal at an arrow, direct multiplication of the reflection matrices gives

$$
C=-U^{-1}U^{\mathsf T},\qquad I-C=U^{-1}(U+U^{\mathsf T})=U^{-1}B.
$$

Thus $C$ has no fixed vector. It is an integral isometry of a positive definite form, so it has finite order $h$: the image of each lattice [basis vector](../../../../../basis-vector.md) lies in a finite set of vectors of the same norm, giving only finitely many possible isometries. Since $C^h=I$ and $I-C$ is invertible,

$$
I+C+\cdots+C^{h-1}=0.
$$

If an indecomposable survived all $h$ reflection cycles, its dimension vectors $d,Cd,\ldots,C^{h-1}d$ would all be nonzero and componentwise nonnegative, contradicting their zero sum. Therefore it reaches a simple at one of the finitely many reflection steps and is then annihilated. Applying the inverse reflections uniquely reconstructs it from that simple. There are at most $6h$ such stopping positions, proving

$$
\boxed{kQ_3\text{ has finite representation type for every orientation of }E_6.}
$$

This supplies the requested finite-type proof sketch.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
