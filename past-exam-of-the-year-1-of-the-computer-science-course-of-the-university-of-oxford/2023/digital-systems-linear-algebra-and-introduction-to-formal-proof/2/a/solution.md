<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a [message-passing mutual exclusion server](../../../../../message-passing-mutual-exclusion-server.md) with an `owner` field and a [FIFO queue](../../../../../fifo-queue.md). A request includes its client's identity. The server handles one received message at a time, and a client has at most one outstanding request. The following pseudocode assumes reliable [message passing](../../../../../message-passing.md) and compliant clients:
```
owner = NONE
waiting = empty FIFO queue

forever:
    (kind, client) = receive_from_any_client()
    if kind == REQUEST:
        waiting.push_back(client)
    else if kind == RELEASE:
        assert client == owner
        owner = NONE

    if owner == NONE and not waiting.empty():
        owner = waiting.pop_front()
        send(owner, GRANT)
```
A client sends `REQUEST`, waits for `GRANT`, runs its complete animation, and sends `RELEASE` before making another request.

The invariant proving [mutual exclusion](../../../../../mutual-exclusion.md) is: **at most one client has received an unreturned grant, and that client is `owner`.** Only the final block issues a grant, and it first requires no current owner. A valid release removes that ownership. Since clients use the display only while holding a grant, simultaneous use is impossible. The [FIFO queue](../../../../../fifo-queue.md) prevents accepted requests from being overtaken by later ones. With eventual message delivery, continued server execution, and finite animations, each accepted request is eventually served; these progress assumptions are separate from the safety invariant.

## ↑ Ancestors (13)

1. [A](../a.md)
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
