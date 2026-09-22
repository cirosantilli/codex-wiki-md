<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use a customer object with no selected platforms as the base component, and wrap it once for each selected channel. Each [decorator object](../../../../../decorator-object.md) has the same interface, delegates existing work, adds one platform send, and adds that platform's per-message charge. The code below uses the `Customer` and `Comms` interfaces from the question; every decorator receives the communication implementation explicitly.

```
final class NoChannels(val name: String) extends Customer {
  def spread(msg: String): Unit = ()
  def cost: Double = 0.0
}

abstract class CustomerDecorator(protected val inner: Customer)
    extends Customer {
  final val name: String = inner.name
  def spread(msg: String): Unit = inner.spread(msg)
  def cost: Double = inner.cost
}

final class OnDiscord(c: Customer, out: Comms)
    extends CustomerDecorator(c) {
  override def spread(msg: String): Unit = {
    super.spread(msg)
    out.sendD(name, msg)
  }
  override def cost: Double = super.cost + 0.01
}

final class OnFacebook(c: Customer, out: Comms)
    extends CustomerDecorator(c) {
  override def spread(msg: String): Unit = {
    super.spread(msg)
    out.sendF(name, msg)
  }
  override def cost: Double = super.cost + 0.05
}

final class OnWhatsApp(c: Customer, out: Comms)
    extends CustomerDecorator(c) {
  override def spread(msg: String): Unit = {
    super.spread(msg)
    out.sendW(name, msg)
  }
  override def cost: Double = super.cost + 0.03
}

def customer(name: String, discord: Boolean, facebook: Boolean,
             whatsapp: Boolean, out: Comms): Customer = {
  var c: Customer = new NoChannels(name)
  if (discord) c = new OnDiscord(c, out)
  if (facebook) c = new OnFacebook(c, out)
  if (whatsapp) c = new OnWhatsApp(c, out)
  c
}
```

The factory admits each platform at most once, matching a subset of preferences. For example, `customer("reader", true, false, true, out)` sends once to Discord and once to WhatsApp and has **cost $0.04$ per message**, using the stipulated charges. The innermost wrapper executes first, giving deterministic Discord–Facebook–WhatsApp order for selected channels. The zero-platform case sends nothing and costs zero. Repeated messages reuse the same immutable choice of wrappers.

By [structural induction](../../../../../structural-induction.md) on the wrapper chain, the base sends to the empty subset with zero cost; one additional wrapper preserves all prior sends and adds exactly its channel and charge. Thus **the sends and charge are composed from the same selected components**. There are $P$ channel-specific classes instead of one class per subset, and a new channel needs one new wrapper. A direct manual construction containing the same wrapper twice would intentionally send and charge twice, so the factory prevents that configuration. `cost` computes a per-message amount rather than charging by itself; a later payment mechanism can use it. The interface uses `Double`, so numerical tests should allow ordinary [floating-point rounding](../../../../../floating-point-rounding.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
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
