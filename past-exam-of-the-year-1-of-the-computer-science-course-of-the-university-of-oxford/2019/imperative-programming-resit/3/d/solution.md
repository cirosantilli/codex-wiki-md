<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Start with a private permanent header whose `next` is null. Its two [string](../../../../../string.md) fields are ignored. For a concrete state satisfying the [representation invariant](../../../../../representation-invariant.md), define the [abstraction function](../../../../../abstraction-function.md)

$$
\alpha(header)=\{v.name\mapsto v.number:\ v\text{ is a real node reachable from }header.next\}.
$$

The [representation invariant](../../../../../representation-invariant.md) says that the header exists, the reachable real [linked list](../../../../../linked-list.md) is finite and acyclic, the header is not a real reachable [linked list node](../../../../../linked-list-node.md), all real name/number fields are non-null [strings](../../../../../string.md), and real names are pairwise distinct. The real [linked list nodes](../../../../../linked-list-node.md) are owned by the book, so clients cannot mutate their fields through exposed references. Distinct names ensure that the displayed relation is a [partial function](../../../../../partial-function.md). The initial empty [linked list](../../../../../linked-list.md) has abstraction $\varnothing$. Reordering real [linked list nodes](../../../../../linked-list-node.md) changes the representation but not the abstract book.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [Imperative programming resit](../../../imperative-programming-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
