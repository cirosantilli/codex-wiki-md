<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose a fixed positive capacity $C$ and represent the abstract state by a finite [partial function](../../../../../partial-function.md) $rep:\mathbb Z\rightharpoonup\mathbb Z$. Its [domain of a partial function](../../../../../domain-of-a-partial-function.md) $S$ has at most $C$ members; each $rep(x)$ belongs to $S$ and is a fixed point:

$$
rep(rep(x))=rep(x)\qquad(x\in S).
$$

The [blocks of a set partition](../../../../../block-of-a-set-partition.md) are the nonempty fibres of `rep`, and their shared values are their [disjoint-set representatives](../../../../../disjoint-set-representative.md). Initially **$rep=\varnothing$**, so $S=\varnothing$. Representatives need not be the minimum members of their blocks.

```
trait DisjointSets {
  val capacity: Int
  // State: rep is a finite idempotent map, |dom rep| <= capacity.
  // Initially: rep is empty; capacity is fixed and positive.

  // Pre: x is absent and |dom rep| < capacity.
  // Post: add x -> x; leave every old mapping unchanged.
  def makeSet(x: Int): Unit

  // Pre: x belongs to dom rep.
  // Post: state unchanged; return rep(x).
  def find(x: Int): Int

  // Pre: x and y belong to dom rep.
  // Post: merge their blocks, retaining old rep(x).
  def union(x: Int, y: Int): Unit
}
```

Precisely, `makeSet(x)` extends the [domain of a partial function](../../../../../domain-of-a-partial-function.md) by $x$ with $rep'(x)=x$. For `union(x,y)`, snapshot $r_x=rep_0(x)$ and $r_y=rep_0(y)$, keep $S$ unchanged, and set

$$
rep'(z)=\begin{cases}r_x&rep_0(z)=r_y,\\rep_0(z)&\text{otherwise}.\end{cases}
$$

This merges the two blocks and keeps the representative of the first argument's block. If $r_x=r_y$, it is an identity operation. This deterministic design choice satisfies [disjoint set union](../../../../../disjoint-set-data-structure.md) without imposing minimum-element representatives. The capacity bound is explicit in the [abstract data type](../../../../../abstract-data-type.md) so that the bounded implementation does not silently strengthen `makeSet`'s [precondition](../../../../../precondition.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
