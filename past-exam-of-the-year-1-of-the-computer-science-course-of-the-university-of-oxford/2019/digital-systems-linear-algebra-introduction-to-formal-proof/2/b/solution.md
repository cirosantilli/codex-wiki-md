<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**Maintain a counter and independent timed [finite-state machine](../../../../../finite-state-machine.md) for each detector–light pair, while sharing the [interrupt](../../../../../interrupt.md) scan and timer infrastructure.** Blocking for one channel's flash would unnecessarily delay every other channel.

```
eye_handler():
    for i in all_channels:
        if EYE_DETECTED[i] != 0:
            EYE_DETECTED[i] = 0
            pending[i] = pending[i] + 1

main_event_loop():
    initialise each LIGHT[i] = 0
    initialise pending[i] = 0, state[i] = IDLE
    enable detector interrupts
    forever:
        now = monotonic_timer_snapshot()
        for i in all_channels:
            service_channel(i, now)
        arrange the next wake-up for new work or the earliest deadline
```

`service_channel` is the three-state sequencer from (a), with its own `started[i]` and an interrupt-safe `try_take_event(i)`. [Shared interrupt demultiplexing](../../../../../shared-interrupt-demultiplexing.md) uses separate `if` tests, not an `else if` chain: simultaneous pending detectors must all be acknowledged and counted. If a new detector becomes pending during the scan, the controller must retrigger while a flag remains set or the handler must rescan appropriately; the exact [interrupt controller](../../../../../interrupt-controller.md) semantics must be checked rather than assuming a single scan can never miss an edge.

One [hardware timer](../../../../../hardware-timer.md) can schedule the earliest active channel deadline. On its expiry, service every due channel and rearm for the next deadline; a periodic tick with adequate resolution is a simpler alternative. Detectors and the timer can then interleave without serial one-second waits. The handler/main-program counter accesses need the same short [critical section](../../../../../critical-section.md) protection as in (a). Keep timing state in one execution context, or protect it too if both a timer handler and the main program modify it.

The [loop invariants](../../../../../loop-invariant.md) are per channel: the pending count equals recorded but unstarted events, `ON` means that channel's light is on, and `GAP` prevents a new flash until one second after its preceding light-off transition. Different channels may flash simultaneously. The [event latch](../../../../../single-bit-event-latch.md) rearming limitation, finite backlog capacity and timer-resolution qualifications apply independently to each channel. These cannot be solved by replacing several [event counters](../../../../../event-counter.md) with one global [Boolean variable](../../../../../boolean-variable.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
