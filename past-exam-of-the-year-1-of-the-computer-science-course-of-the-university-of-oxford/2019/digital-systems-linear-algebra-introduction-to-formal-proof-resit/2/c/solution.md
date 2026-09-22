<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Safety:** only the driver accesses the sensor, and `active` identifies at most one conversion. Accepted requests are serialized by the [FIFO queue](../../../../../fifo-queue.md). The reply destination and token identify the owner of the resulting sample; no caller can clear another conversion's ready flag or consume another result. Receiving new requests while busy only changes the queue, not the active measurement. These are [mutual exclusion](../../../../../mutual-exclusion.md) and request/result association properties, not timing guesses.

**Progress:** assume each started conversion completes in finite time, the corresponding notification is eventually delivered, the driver and compliant clients are eventually scheduled, and pending message acceptance is fair. A caller remains ready to receive its reply. Every accepted request has finitely many earlier requests in the queue, and later arrivals cannot overtake it. Each earlier request is completed and removed in finite time, so the caller eventually becomes active and receives its own reading. Fair acceptance extends this argument from accepted requests to callers waiting to submit one.

These assumptions are necessary for [starvation freedom](../../../../../starvation-freedom.md). A failed sensor, a client that disappears before accepting a synchronous reply, or an unfair scheduler can prevent progress; serialization alone cannot prove otherwise. Under the stated operating model, simultaneous calls are safe and every call completes. A single shared “latest temperature” variable would not establish either a fresh conversion per call or correct reply ownership.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
