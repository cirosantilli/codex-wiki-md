<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

A [metric space](../../../../../metric-space.md) is a set $X$ with a nonnegative symmetric distance $d$, zero exactly for equal points, satisfying $d(x,z)\leq d(x,y)+d(y,z)$. A [Cauchy sequence](../../../../../cauchy-sequence.md) is a sequence for which, given any $\epsilon>0$, there is $N$ such that $d(x_n,x_m)<\epsilon$ whenever $n,m\geq N$.

For a [pseudometric](../../../../../pseudometric.md), zero distance defines an [equivalence relation](../../../../../equivalence-relation.md). Reflexivity and symmetry are immediate; transitivity follows from $d(x,z)\leq d(x,y)+d(y,z)=0$ when both terms vanish. Define $d_Q([x],[y])=d(x,y)$. If $x\sim x'$ and $y\sim y'$, the triangle inequality gives $d(x,y)\leq d(x',y')$ and its reversed version gives equality. Thus the definition is independent of representatives. The nonnegative, symmetric and triangle properties descend, while zero distance means precisely that the two classes are equal. It is therefore a [metric quotient of a pseudometric](../../../../../metric-quotient-of-a-pseudometric.md).

Now take two [Cauchy sequences](../../../../../cauchy-sequence.md) in the original metric space. Two applications of the triangle inequality give

$$
|d(x_n,y_n)-d(x_m,y_m)|\leq d(x_n,x_m)+d(y_n,y_m).
$$

The right-hand side is arbitrarily small when both indices are large, so $(d(x_n,y_n))$ is a real Cauchy sequence and has a finite real limit. Consequently

$$
\overline d((x_n),(y_n))=\lim_n d(x_n,y_n)
$$

is well defined. Nonnegativity, symmetry and zero self-distance follow by passing to the limit in the corresponding properties of $d$. Passing to the limit in $d(x_n,z_n)\leq d(x_n,y_n)+d(y_n,z_n)$ gives its triangle inequality. Thus $\overline d$ is a pseudometric on $C$, and the preceding quotient construction makes $C/R$ a metric space.

Map $x\in X$ to the class of its constant sequence. The distance between two such classes is $d(x,y)$, so this is an injective [isometric embedding](../../../../../isometric-embedding.md). It is surjective exactly when every Cauchy sequence $(x_n)$ is equivalent to a constant sequence $(x)$, that is, when $d(x_n,x)\to0$ for some $x\in X$. This is precisely [completeness](../../../../../completeness.md). Hence

$$
\boxed{X\longrightarrow C/R\text{ is bijective if and only if }X\text{ is complete}.}
$$

The quotient is the [Cauchy-sequence construction of a metric completion](../../../../../cauchy-sequence-construction-of-a-metric-completion.md); the conclusion requires no assumption that $X$ is compact.

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
