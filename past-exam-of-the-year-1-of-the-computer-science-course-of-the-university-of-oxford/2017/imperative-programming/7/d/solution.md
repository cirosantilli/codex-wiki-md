<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Replace the overloaded entry family by one forwarding method and introduce the second dispatch explicitly:

```
class X {
  def dispatch(to: M): String = to.visit(this)
}
class Y extends X {
  override def dispatch(to: M): String = to.visit(this)
}
class Z extends Y {
  override def dispatch(to: M): String = to.visit(this)
}

class M {
  def f(x: X): String = x.dispatch(this)
  def visit(x: X): String = "f with X at M"
  def visit(x: Y): String = "f with Y at M"
  def visit(x: Z): String = "f with Z at M"
}
class N extends M {
  override def visit(x: X): String = "f with X at N"
  override def visit(x: Y): String = "f with Y at N"
  override def visit(x: Z): String = "f with Z at N"
}
```

The original three calls still type-check because all their arguments are subtypes of `X`. They all refer to the same runtime `Z` object already; the change is how the operation discovers that runtime type. The first virtual call selects `Z.dispatch`, where `this` has static type `Z`, so overload resolution selects `visit(Z)`. The second virtual call selects `N.visit(Z)` from the receiver's runtime type. Thus [double dispatch](../../../../../double-dispatch.md) gives **`f with Z at N` on all three lines**.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
