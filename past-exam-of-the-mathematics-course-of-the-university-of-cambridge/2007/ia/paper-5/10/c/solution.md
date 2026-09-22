<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Add a public override of `toString` in each concrete subclass. In `TypeVar`:
```
public String toString() {
    return "t" + id.toString();
}
```
In `Arrow`:
```
public String toString() {
    return "(" + from.toString() + " -> " + to.toString() + ")";
}
```
Inherited dynamic dispatch selects the proper method at every node of the [abstract syntax tree](../../../../../../abstract-syntax-tree.md). Full parentheses distinguish the domain and codomain nesting without relying on a reader's precedence convention. Repeated occurrences of one [type variable](../../../../../../type-variable.md) use the same identifier, and distinct factory variables have distinct identifiers. For example, with the first three factory variables, the type from part (b) prints as `((t1 -> t2) -> (t2 -> t3))`. **The recursive textual form preserves both arrow structure and variable identity.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10](../../10.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
