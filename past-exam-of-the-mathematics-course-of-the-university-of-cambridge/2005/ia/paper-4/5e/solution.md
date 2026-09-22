<h1 id="5e/solution">Solution</h1>

↑ **Parent:** [5E](../5e.md)

A [countable set](../../../../../countable-set.md) is a set that is finite or can be put in [bijection](../../../../../bijection.md) with the [natural numbers](../../../../../natural-number.md); equivalently, it admits an [injective function](../../../../../injective-function.md) into the natural numbers. To enumerate the [rational numbers](../../../../../rational-number.md), list pairs $(p,q)$ with $p\in\mathbb Z$, $q\ge1$ in increasing order of $|p|+q$, and then list $p/q$, discarding repetitions. Each level is finite and every rational eventually appears. An enumeration $q_1,q_2,\ldots$ of the rationals then enumerates $\mathbb Q\times\mathbb Q$ by listing $(q_i,q_j)$ in diagonals of constant $i+j$. Thus

$$
\boxed{\mathbb Q\times\mathbb Q\text{ is countable}.}
$$

To prove that the [real numbers](../../../../../real-number.md) are [uncountable](../../../../../uncountable-set.md), suppose $(0,1)$ had an enumeration $x_1,x_2,\ldots$. Write each $x_n$ in its decimal expansion that does not end in an infinite string of nines. Define a new decimal $y=0.d_1d_2\cdots$ by taking $d_n=2$ if the $n$th digit of $x_n$ is $1$, and $d_n=1$ otherwise. Then $y\in(0,1)$, has no ambiguous terminating/nines representation, and differs from $x_n$ at digit $n$. The [Cantor diagonal argument](../../../../../cantor-diagonal-argument.md) contradicts the supposed enumeration. Consequently **the real numbers are uncountable**.

For the discs, use the enumeration of $\mathbb Q^2$ just constructed. Every positive-radius disc contains a rational-coordinate point: its interior contains a small open rectangle, and each coordinate interval contains a rational number. For each disc $D$, let $j(D)$ be the least index of an enumerated rational-coordinate point in its interior. This minimum exists and requires no arbitrary simultaneous choice. Disjoint discs cannot receive the same point, so $D\mapsto j(D)$ is an [injective function](../../../../../injective-function.md) into the natural numbers. This proves the [countability of pairwise disjoint open disks](../../../../../countability-of-pairwise-disjoint-open-disks.md) and also the same conclusion for closed discs, by using their disjoint interiors.

For circles, take all concentric [circles](../../../../../circle.md) centred at the origin with radii $r\in(1,2)$. Two different radii give disjoint [circles](../../../../../circle.md), and every radius is positive. The radius map is a [bijection](../../../../../bijection.md) from the uncountable interval $(1,2)$ to this family. **An uncountable disjoint family of nontrivial circles is therefore possible:** the rational-point argument for discs relies on their nonempty interiors, which circumferences do not have.

## ↑ Ancestors (10)

1. [5E](../5e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
