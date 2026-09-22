<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [double dispatch](../../../../../double-dispatch.md). Each original overload first sends a dynamically dispatched message to its argument. The argument's selected body then calls an overloaded receiver method with `this`, whose [static type](../../../../../static-type.md) inside that body is the desired argument [software class](../../../../../class-programming.md).
```
class X {
  def sendTo(m: M): String = m.receive(this)
}
class Y extends X {
  override def sendTo(m: M): String = m.receive(this)
}
class Z extends Y {
  override def sendTo(m: M): String = m.receive(this)
}

class M {
  def f(x: X): String = x.sendTo(this)
  def f(x: Y): String = x.sendTo(this)

  def receive(x: X): String = "f with X at M"
  def receive(x: Y): String = "f with Y at M"
  def receive(x: Z): String = "f with Z at M"
}

class N extends M {
  override def f(x: Y): String = x.sendTo(this)
  def f(x: Z): String = x.sendTo(this)

  override def receive(x: X): String = "f with X at N"
  override def receive(x: Y): String = "f with Y at N"
  override def receive(x: Z): String = "f with Z at N"
}
```
All three `receive` overloads must be declared in `M`, because `sendTo` receives a parameter with [static type](../../../../../static-type.md) `M`. Declaring the `Z` version only in `N` would repeat the original problem.

Whatever original `f` signature is selected, it invokes `sendTo` on the actual argument. For a `Z` object, [dynamic dispatch](../../../../../dynamic-dispatch.md) enters `Z.sendTo`; inside that body, `this` has [static type](../../../../../static-type.md) `Z`, so [method overloading](../../../../../method-overloading.md) selects `receive(Z)`. The final call dynamically dispatches on the actual `m`, giving `N.receive(Z)` when `m` refers to `N`. Hence
```
f with Z at N
f with Z at N
f with Z at N
```
The result depends on both [runtime types](../../../../../runtime-type.md):

$$
\boxed{\text{argument }Z\text{ selects }receive(Z),\qquad\text{receiver }N\text{ selects its override}.}
$$

For the stated `X`, `Y`, `Z` hierarchy, the same construction reports each argument [software class](../../../../../class-programming.md) correctly for either receiver [software class](../../../../../class-programming.md). Further subclasses would need their own dispatch protocol to distinguish additional [runtime types](../../../../../runtime-type.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
