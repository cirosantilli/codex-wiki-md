<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Suppose the weak-star closure of $Z$ were a proper linear [vector subspace](../../../../../../vector-subspace.md) of $X^*$. The [Hahn-Banach separation theorem](../../../../../../hahn-banach-separation-theorem.md) would give a nonzero weak-star [continuous linear functional](../../../../../../continuous-linear-functional.md) vanishing on it. A [continuous dual of a weak-star topology](../../../../../../continuous-dual-of-a-weak-star-topology.md) consists precisely of evaluations at points of $X$: [continuity](../../../../../../continuous-function.md) bounds the [linear functional](../../../../../../linear-functional.md) by finitely many evaluations, so it factors through their finite-dimensional coordinate map and is a linear combination of them. Thus some $0\neq x\in X$ would satisfy $z(x)=0$ for all $z\in Z$. The norming inequality would imply $c\|x\|\leq0$, a contradiction. **Every [norming subspace](../../../../../../norming-subspace-of-a-dual-space.md) of $X^*$ is weak-star dense.**

For the infinite-codimension example, take

$$
\boxed{X=\ell^1(\mathbb N;\mathbb R),\qquad X^*=\ell^\infty(\mathbb N;\mathbb R),\qquad Z=c_0.}
$$

Here $X$ is the [absolutely summable sequence space](../../../../../../absolutely-summable-sequence-space.md) and $c_0$ is the [space of sequences converging to zero](../../../../../../space-of-sequences-converging-to-zero.md), a norm-closed [vector subspace](../../../../../../vector-subspace.md) of $\ell^\infty$. The dual identification is $y(x)=\sum_nx_ny_n$: a bounded sequence defines a [linear functional](../../../../../../linear-functional.md) of [norm](../../../../../../norm.md) $\|y\|_\infty$, and every [linear functional](../../../../../../linear-functional.md) on $\ell^1$ has this form by evaluating on the coordinate vectors and using density of finitely supported sequences.

For $x\in\ell^1$, use the finitely supported sequence $y^{(N)}$ whose first $N$ entries are $\operatorname{sgn}(x_n)$ and whose remaining entries vanish. It belongs to $c_0$, has [norm](../../../../../../norm.md) at most one, and

$$
y^{(N)}(x)=\sum_{n=1}^N|x_n|\longrightarrow\|x\|_1.
$$

The reverse inequality follows from $|y(x)|\leq\|y\|_\infty\|x\|_1$. Hence **$c_0$ is 1-norming for $\ell^1$**, an instance of [vanishing sequences norm the summable sequence space](../../../../../../vanishing-sequences-norm-the-summable-sequence-space.md).

To prove infinite codimension, take disjoint infinite sets

$$
A_j=\{2^{j-1}(2m-1):m\geq1\},\qquad j\geq1.
$$

Their indicator sequences have linearly independent classes in $\ell^\infty/c_0$. Indeed, a finite combination has the constant value $a_j$ on $A_j$; if it tends to zero, every $a_j$ must vanish. Thus the quotient is infinite-dimensional.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
