<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The two writable inputs and Boolean query belong to an [abstract class](../../../../../abstract-class.md); each concrete [logic gate](../../../../../logic-gate.md) overrides just that query:
```
abstract class Gate {
  var inp1: Boolean = false
  var inp2: Boolean = false
  def evalGate: Boolean
}

class OrG extends Gate {
  override def evalGate: Boolean = inp1 || inp2
}

class AndG extends Gate {
  override def evalGate: Boolean = inp1 && inp2
}

class XorG extends Gate {
  override def evalGate: Boolean = inp1 ^ inp2
}
```
All three subclasses satisfy the same [object interface](../../../../../object-interface.md), so the `Gate` declarations in the supplied simulator still allow access to inputs and invoke the correct [Boolean function](../../../../../boolean-function.md) through [dynamic dispatch](../../../../../dynamic-dispatch.md). Boolean `^` is [exclusive or](../../../../../exclusive-or.md); `||` is [Boolean disjunction](../../../../../logical-disjunction.md) and `&&` is [Boolean conjunction](../../../../../logical-conjunction.md).

The program first sets both inputs of `y`, so $y=\mathrm{true}\land\mathrm{true}=\mathrm{true}$. It sets $z=\mathrm{false}\mathbin{\mathrm{xor}}\mathrm{false}=\mathrm{false}$. Therefore $x=y\lor z=\mathrm{true}$ and $w=z\land\mathrm{true}=\mathrm{false}$, giving
```
x: true
w: false
```
**Those are the two output lines.** This is a simulation of [combinational logic](../../../../../combinational-logic.md) in an order where each gate's inputs have already been calculated; the Boolean assignments copy values rather than create live wire connections.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
