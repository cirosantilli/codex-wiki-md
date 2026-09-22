<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Give the hardware to a single [device driver](../../../../../device-driver.md) process. Other processes request a conversion through [message passing](../../../../../message-passing.md) and never touch its [memory-mapped input-output](../../../../../memory-mapped-input-output.md) registers. The following is protocol pseudocode for [Phōs](../../../../../phos.md): its operation names specify their required semantics, rather than asserting an unverified spelling of a particular 2019 C interface. The hardware actions and the request/reply design are fully specified.

Use a [FIFO queue](../../../../../fifo-queue.md) of accepted requests, each containing its sender and a per-call token. Bind the device's interrupt to a persistent notification addressed to the driver before any conversion is started. A notification must remain pending if it arrives before the driver next waits; this is the [lost-wakeup avoidance](../../../../../lost-wakeup-avoidance.md) requirement. The driver receives both client requests and interrupt notifications in its event loop.

```
configure sensor and connect its interrupt notification to this process
TEMP_DATARDY := 0
clear stale pending interrupt notification
enable sensor interrupt and interrupt-controller delivery
pending := empty FIFO
active := none

forever:
    if active is none and pending is not empty:
        active := remove oldest request from pending
        TEMP_DATARDY := 0
        clear stale pending interrupt notification
        TEMP_START := 1

    event := wait for a request or persistent interrupt notification

    if event is REQUEST(sender, token):
        append (sender, token) to pending

    if event is sensor interrupt and active is not none:
        if TEMP_DATARDY != 0:
            value := TEMP_TEMP
            TEMP_DATARDY := 0
            acknowledge the interrupt through the OS interrupt mechanism
            send RESULT(active.token, value) to active.sender
            active := none
```

After receiving an idle-time request, the next loop iteration starts its conversion before waiting again. While a conversion is in progress, additional requests join the queue without starting another conversion. A completed reading is copied before its ready flag is cleared, and the next request cannot start until the current result has been delivered. Spurious or stale notifications do not complete a request unless the device's ready register confirms completion.

Clearing old status and notification precedes `TEMP_START`; doing so afterwards could erase a very fast completion. The [operating system](../../../../../operating-system-split.md) interrupt binding and persistent notification cover completion in the interval between starting the device and entering the wait. Register accesses must use the platform's device-access semantics, including required [volatile-qualified objects in C](../../../../../volatile-qualified-objects-in-c.md) or ordering primitives. Exact initialization and interrupt-connection call names remain an implementation binding, not invented [Phōs](../../../../../phos.md) API calls. The later teaching site's named system is documented separately; it is not used as [proof](../../../../../mathematical-proof.md) of an identical historical API.[2018–2019 course record and linked teaching-site description of process/message-based device drivers](../../../../../digital-systems-course-archive-of-the-university-of-oxford.md)

## ↑ Ancestors (12)

1. [A](../a.md)
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
