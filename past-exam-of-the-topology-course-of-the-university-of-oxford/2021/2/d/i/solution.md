<h1 id="2/d/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

Use positive indices $n\geq1$ and write $p=(0,-1)\in S^1$. Set

$$
\boxed{A=\mathbb N\times\{p\},\qquad f(n,(u,v))=\left(\frac un,\frac{v+1}{n}\right).}
$$

For fixed $n$, this [function](../../../../../function-split.md) is a [homeomorphism](../../../../../homeomorphism.md) from the [unit circle](../../../../../complex-unit-circle.md) to $C_n$: it scales its [radius](../../../../../radius.md) to $1/n$ and translates its centre to $(0,1/n)$. Thus it takes values in the [Hawaiian earring](../../../../../hawaiian-earring.md) $X$ and is [surjective](../../../../../surjective-function.md) onto $X$. It is [continuous](../../../../../continuous-function.md) on each [open](../../../../../open-set.md) slice $\{n\}\times S^1$; since these slices form an [open cover](../../../../../open-cover.md) of $\mathbb N\times S^1$, $f$ is [continuous](../../../../../continuous-function.md) on the whole [product topology](../../../../../product-topology.md).

Distinct [circles](../../../../../circle.md) $C_n,C_m$ meet only at $o=(0,0)$. To see this directly, their equations are

$$
x^2+y^2=\frac{2y}{n},\qquad x^2+y^2=\frac{2y}{m}.
$$

For $m\neq n$, subtraction gives $y=0$, then $x=0$. Each slice contains exactly one [preimage](../../../../../preimage.md) of $o$, namely $(n,p)$. Therefore the only nonsingleton [fibre](../../../../../fiber-of-a-function.md) of $f$ is $A$.

Let $q:\mathbb N\times S^1\to(\mathbb N\times S^1)/A$ be the [quotient map](../../../../../quotient-map.md) collapsing $A$. The [universal property of the quotient topology](../../../../../universal-property-of-the-quotient-topology.md) supplies a unique [continuous map](../../../../../continuous-map.md) $\bar f$ with $f=\bar f\circ q$. The [fibre](../../../../../fiber-of-a-function.md) calculation proves [injectivity](../../../../../injective-function.md), and [surjectivity](../../../../../surjective-function.md) follows from that of $f$. Hence **$\bar f$ is the required [continuous bijection](../../../../../continuous-bijection.md)**.

## ↑ Ancestors (13)

1. [i](../i.md)
2. [d](../../d.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the topology course of the University of Oxford](../../../../split.md)
6. [Topology course of the University of Oxford](../../../../../topology-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
