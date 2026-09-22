<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use two [FIFO queues](../../../../../fifo-queue.md), one for each priority class, and perform [nonpreemptive strict-priority arbitration](../../../../../nonpreemptive-strict-priority-arbitration.md) whenever the display becomes free:
```
owner = NONE
ordinary = empty FIFO queue
urgent = empty FIFO queue

forever:
    message = receive_from_any_client()
    if message.kind == REQUEST:
        assert message.priority in {0, 1}
        if message.priority == 1:
            urgent.push_back(message.client)
        else:
            ordinary.push_back(message.client)
    else if message.kind == RELEASE:
        assert message.client == owner
        owner = NONE

    if owner == NONE:
        if not urgent.empty():
            owner = urgent.pop_front()
        else if not ordinary.empty():
            owner = ordinary.pop_front()
        if owner != NONE:
            send(owner, GRANT)
```
The same ownership invariant proves [mutual exclusion](../../../../../mutual-exclusion.md). Among requests already accepted by the server, every pending urgent request takes precedence over every ordinary one. Each class retains its own arrival order. A newly received urgent request goes ahead of waiting ordinary requests but waits for the current animation's `RELEASE`; the given protocol has no interruption or revocation operation.

This is strict priority at dispatch, based on requests the server has received. Requests still in transit cannot influence a decision. If the transport provides a mailbox-draining operation, the server may also collect all currently delivered requests before dispatching; the two-[FIFO queue](../../../../../fifo-queue.md) selection rule remains the same.

Strict priority does not guarantee [starvation freedom](../../../../../starvation-freedom.md) for ordinary clients under an endless supply of urgent work. If urgent traffic eventually stops, accepted requests have only finitely many earlier requests, and all service times are finite, every pending ordinary request is eventually granted. Guaranteeing ordinary progress under unlimited urgent traffic would require a different fairness policy, such as limiting consecutive urgent grants; that would relax strict priority.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [Digital systems](../../digital-systems.md)
4. [Digital systems, linear algebra and introduction to formal proof](../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
5. [2023](../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
