<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [directed graph](../../../../../../directed-graph.md) needs an explicit termination argument. After assigning its [parent in a rooted tree](../../../../../../parent-in-a-rooted-tree.md), a [vertex](../../../../../../vertex-graph-theory.md) must still receive later traffic: having no new [graph neighbours](../../../../../../neighbour-of-a-vertex.md) to discover is not proof that other senders have finished. Use a discovery wave together with duplicate-suppressed announcements of activated [vertices](../../../../../../vertex-graph-theory.md). Both kinds of message identify their immediate sender, who has already activated.

```
sealed trait Msg { def from: NodeId }
final case class Discover(from: NodeId) extends Msg
final case class Active(from: NodeId, origin: NodeId) extends Msg
```

Let `adj = neighbours.distinct`. The actual communication objects must expose both input and output ports: the paper's `Seq[![Msg]]` annotation supplies only output capabilities, although the following sentence also requires receiving. Set up one shared-writer, single-reader buffered [message-passing channel](../../../../../../message-passing-channel.md) per [vertex](../../../../../../vertex-graph-theory.md), publish its output in `toNode`, and keep its input in `fromNode`. Only node `i` reads `fromNode(i)`. These are the two ports of the same underlying mailbox, not additional [graph edges](../../../../../../edge-of-a-graph.md). The question's prohibition on buffered [message-passing channels](../../../../../../message-passing-channel.md) applies to Question 1(a), not to this question.

Take $N\geq1$, reliable delivery, eventual scheduling, finite `adj`, and mailbox capacity $B=N(N+1)$. Every node has at most $N$ distinct incoming neighbours, including itself if there is a self-loop. The bound below ensures that no send blocks merely because a mailbox's receiver is not currently reading. Do not close these shared mailboxes on local process termination: late, redundant traffic is harmless and bounded. Their creator can release them after the parallel composition has joined. For example, the concrete setup can use

```
val mailbox = Vector.fill(N)(N2NBuf[Msg](B, 0, 1))
val toNode: Seq[![Msg]] = mailbox
val fromNode: Seq[?[Msg]] = mailbox
```

Here the zero writer count makes the shared output independent of individual writer departures; processes do not call its `closeOut` during the search.

```
def span: PROC = proc {
  val adj = neighbours.distinct
  var started = false
  val known = scala.collection.mutable.Set[NodeId]()

  def announce(origin: NodeId): Unit = {
    if (!known(origin)) {
      known += origin
      for (w <- adj) toNode(w) ! Active(me, origin)
    }
  }
  def activate(sender: NodeId): Unit = {
    started = true
    parent = if (me == 0) 0 else sender
    for (w <- adj if me == 0 || w != parent)
      toNode(w) ! Discover(me)
    announce(me)
  }

  if (me == 0) activate(0)
  while (known.size < N) {
    val message = fromNode(me) ? ()
    if (!started) activate(message.from)
    message match {
      case Discover(_) => ()
      case Active(_, origin) => announce(origin)
    }
  }
}
```

An announcement may be a [vertex](../../../../../../vertex-graph-theory.md)'s first incoming message. It then serves as a discovery message too: its immediate sender is already active, and the receiving [vertex](../../../../../../vertex-graph-theory.md) adopts that sender as its [parent in a rooted tree](../../../../../../parent-in-a-rooted-tree.md) before forwarding anything. This preserves the required first-message rule. In particular, an inactive [vertex](../../../../../../vertex-graph-theory.md) never forwards announcements while remaining inactive, which could invalidate the parent-order argument.

For each nonroot [vertex](../../../../../../vertex-graph-theory.md), its [parent in a rooted tree](../../../../../../parent-in-a-rooted-tree.md) activated strictly earlier. Repeated parent-following therefore cannot make a [graph cycle](../../../../../../cycle-in-a-graph.md) and eventually reaches the unique initially active [vertex](../../../../../../vertex-graph-theory.md), zero. Each parent assignment uses an actual incoming [directed edge](../../../../../../directed-edge.md). [Strong connectivity](../../../../../../strong-connectivity.md) ensures eventual activation of every [vertex](../../../../../../vertex-graph-theory.md): if an activated set were proper, a [directed path](../../../../../../directed-path.md) from zero to an inactive [vertex](../../../../../../vertex-graph-theory.md) would have a first edge leaving that set. Its sender sends a discovery message along that edge; excluding its own parent does not exclude an inactive neighbour.

Each activation sends at most one `Discover` on each outgoing [directed edge](../../../../../../directed-edge.md). For each of the $N$ origins, each [vertex](../../../../../../vertex-graph-theory.md) forwards `Active` at most once on each outgoing [directed edge](../../../../../../directed-edge.md). Therefore a mailbox receives at most $N(N+1)$ messages over the whole run, proving the chosen nonblocking storage bound. Each origin's announcement eventually reaches every [vertex](../../../../../../vertex-graph-theory.md), since every first receipt forwards it on all outgoing [directed edges](../../../../../../directed-edge.md). Thus every `known` set reaches size $N$ and every process terminates, even if redundant messages remain unread:

$$
\boxed{\mathrm{parent}(0)=0;\quad \mathrm{parent}(v)\text{ is the sender of }v\text{'s first message},\ v\ne0.}
$$

No timeout is used to conclude that the distributed work has finished. This uses larger finite mailboxes to make the termination proof simple, rather than assuming that simultaneous synchronous broadcasts cannot [deadlock](../../../../../../deadlock.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Concurrent programming](../../../../concurrent-programming-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
