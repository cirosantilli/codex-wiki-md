<h1 id="7/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**`Fun[Base, Derived]` can safely supply a `Fun[Base, Base]` contract; `Fun[Base, Base]` cannot in general supply a `Fun[Base, Derived]` contract.** The input obligation is unchanged, while a derived result satisfies every base-result promise. This is the covariant output rule of [function](../../../../../../function-split.md) [subtyping](../../../../../../subtyping.md).

With the invariant printed [trait](../../../../../../trait.md), implement the safe view explicitly:

```
def widenResult(f: Fun[Base, Derived]): Fun[Base, Base] =
  new Fun[Base, Base] {
    def apply(x: Base): Base = f(x)
  }
```

Using the illustrative classes from part i, an unsafe substitution would let a client assume a derived-only operation on a result that is merely a base [software object](../../../../../../software-object.md):

```
val broadResult = new Fun[Base, Base] {
  def apply(x: Base): Base = new Base
}
def derivedResultClient(f: Fun[Base, Derived]): Int =
  f(new Base).special()
// derivedResultClient(broadResult) must be rejected.
```

The direct, variance-aware [object interface](../../../../../../object-interface.md) that would express both safe directions is `trait Fun[-S, +T] { def apply(x: S): T }`. Its [object method](../../../../../../object-method.md) consumes the contravariant parameter and produces the covariant parameter. This is an explicitly proposed variant of the printed invariant declaration, not an assumption that its annotations were already present.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [7](../../../7.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
