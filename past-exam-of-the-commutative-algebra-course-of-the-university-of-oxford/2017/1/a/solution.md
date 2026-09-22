<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [commutative ring](../../../../commutative-ring.md) $R$ is a [Noetherian ring](../../../../noetherian-ring.md) if every [ideal](../../../../ideal.md) has a finite [generating set of an ideal](../../../../generating-set-of-an-ideal.md). Equivalently, it satisfies the [ascending chain condition](../../../../ascending-chain-condition.md) on [ideals](../../../../ideal.md). Indeed, the union of an ascending chain is an [ideal](../../../../ideal.md), and finitely many generators all belong to one term, after which the chain stabilizes. Conversely, an [ideal](../../../../ideal.md) without a finite [generating set of an ideal](../../../../generating-set-of-an-ideal.md) would allow us to choose successively $a_{n+1}\notin(a_1,\ldots,a_n)$, producing a strictly ascending chain of [ideals](../../../../ideal.md).

Let $\phi:R\to S$ be a [surjective](../../../../surjective-function.md) [ring homomorphism](../../../../ring-homomorphism.md), where $R$ is a [Noetherian ring](../../../../noetherian-ring.md). For any [ideal](../../../../ideal.md) $J$ of $S$, its inverse image is an [ideal](../../../../ideal.md) of $R$, say $\phi^{-1}(J)=(a_1,\ldots,a_r)$. Taking images gives

$$
J=(\phi(a_1),\ldots,\phi(a_r)).
$$

Thus [homomorphic images of Noetherian rings are Noetherian](../../../../homomorphic-images-of-noetherian-rings-are-noetherian.md). This also applies to the image of an arbitrary [ring homomorphism](../../../../ring-homomorphism.md), by taking its image as the codomain.

The [Hilbert basis theorem](../../../../hilbert-basis-theorem.md) states that if $R$ is a [Noetherian ring](../../../../noetherian-ring.md), then the [polynomial ring](../../../../polynomial-ring.md) $R[t]$ is a [Noetherian ring](../../../../noetherian-ring.md). Repeating this gives the result for finitely many variables.

To prove it, fix an [ideal](../../../../ideal.md) $K\subseteq R[t]$. For $n\geq0$, define the [coefficient ideals of a polynomial ideal](../../../../coefficient-ideals-of-a-polynomial-ideal.md)

$$
A_n=\{a\in R:\text{some }f\in K\text{ of degree at most }n\text{ has coefficient }a\text{ at }t^n\}.
$$

Here the zero [polynomial](../../../../polynomial-split.md) is allowed. Each $A_n$ is an [ideal](../../../../ideal.md): addition and multiplication by constants preserve the required degree bound. Multiplying a representing [polynomial](../../../../polynomial-split.md) by $t$ gives $A_n\subseteq A_{n+1}$. The [ascending chain condition](../../../../ascending-chain-condition.md) therefore supplies $N$ such that $A_n=A_N$ for every $n\geq N$.

For each $0\leq n\leq N$, choose a finite [generating set of an ideal](../../../../generating-set-of-an-ideal.md) $a_{n1},\ldots,a_{nr_n}$ for $A_n$, omitting zero generators, and choose $f_{nj}\in K$ of [polynomial degree](../../../../degree-of-a-polynomial.md) $n$ with [leading coefficient](../../../../leading-coefficient-of-a-polynomial.md) $a_{nj}$. If $A_n=0$, choose no such [polynomials](../../../../polynomial-split.md). We claim that the finitely many $f_{nj}$ generate $K$.

Take a nonzero $f\in K$ of [polynomial degree](../../../../degree-of-a-polynomial.md) $d$. Put $n=\min(d,N)$. Its [leading coefficient](../../../../leading-coefficient-of-a-polynomial.md) belongs to $A_d=A_n$, so write it as $\sum_jb_ja_{nj}$. The [polynomial](../../../../polynomial-split.md)

$$
g=f-\sum_jb_jt^{d-n}f_{nj}
$$

belongs to $K$ and is either zero or has [polynomial degree](../../../../degree-of-a-polynomial.md) strictly below $d$. Induction on [polynomial degree](../../../../degree-of-a-polynomial.md) now expresses $f$ as a combination of the chosen $f_{nj}$; when $d=0$, the displayed difference is zero. Hence $K$ is finitely generated. Since $K$ was arbitrary, $R[t]$ is a [Noetherian ring](../../../../noetherian-ring.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the commutative algebra course of the University of Oxford](../../../split.md)
5. [Commutative algebra course of the University of Oxford](../../../../commutative-algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
