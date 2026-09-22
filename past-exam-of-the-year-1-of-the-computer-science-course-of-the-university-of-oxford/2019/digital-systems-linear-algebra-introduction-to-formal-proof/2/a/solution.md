<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**A short [interrupt handler](../../../../../interrupt-handler.md) should acknowledge the detector and count work; a timed [finite-state machine](../../../../../finite-state-machine.md) should generate the flashes. A [Boolean](../../../../../boolean-data-type.md) “someone arrived” variable cannot preserve several queued detections.** This is an [interrupt-driven pulse sequencer](../../../../../interrupt-driven-pulse-sequencer.md). Initialise the light off, the pending-event counter to zero and the sequencer to `IDLE` before enabling [interrupts](../../../../../interrupt.md).

In the following pseudocode, [interrupt](../../../../../interrupt.md) acknowledgement uses the source-specified operation of writing zero. The [atomic operation](../../../../../atomic-operation.md) and timer calls name abstract services, not undocumented [device registers](../../../../../device-register.md) of a particular microcontroller.

```
eye_handler():
    if EYE_DETECTED != 0:
        EYE_DETECTED = 0
        pending = pending + 1

try_take_event():
    briefly mask the detector interrupt
    if pending == 0: taken = false
    else: pending = pending - 1; taken = true
    restore the previous interrupt mask
    return taken

service(now):
    if state == ON and elapsed(now, started) >= one_second:
        LIGHT = 0
        state = GAP
        started = now
    if state == GAP and elapsed(now, started) >= one_second:
        state = IDLE
    if state == IDLE and try_take_event():
        LIGHT = 1
        state = ON
        started = now
```

The main program repeatedly handles a new event or the next timer deadline and calls `service`. The `ON` state lasts one second; **every completed flash enters `GAP`, even if the queue is empty at that instant**. An arrival during that gap must wait for it to expire. Otherwise turning the light off and immediately treating the device as idle could allow a new flash too soon. Once a gap has expired, a queued event starts a new flash; if no work is pending the device remains idle. Removing a pending event only when a flash starts gives one completed flash per consumed event.

An [interrupt](../../../../../interrupt.md) can arrive during the main program's decrement. Without a [critical section](../../../../../critical-section.md), its increment can be overwritten by a [race condition](../../../../../race-condition.md). Merely declaring the counter `volatile`, as in [volatile-qualified objects in C](../../../../../volatile-qualified-objects-in-c.md), does not make the decrement an [atomic operation](../../../../../atomic-operation.md). Short [interrupt masking](../../../../../interrupt-masking.md), or an appropriate [atomic operation](../../../../../atomic-operation.md), protects it; [interrupts](../../../../../interrupt.md) must remain enabled during the one-second intervals so that detections continue to be recorded.

A calibrated [busy-wait](../../../../../busy-waiting.md) loop is simple, but occupies the [CPU](../../../../../central-processing-unit.md) and its duration depends on instruction timing, compiler transformations and time spent in [interrupts](../../../../../interrupt.md). Polling a [hardware timer](../../../../../hardware-timer.md) avoids calibration dependence but still consumes [CPU](../../../../../central-processing-unit.md) while polling. A [timer interrupt](../../../../../timer-interrupt.md) or timer comparison deadline permits useful work or safe sleeping between transitions and is preferable for precise timing. If sleeping, the test for queued work and entry into sleep must avoid a [lost wake-up](../../../../../lost-wake-up.md). By the [modulo-counter elapsed-time identity](../../../../../modulo-counter-elapsed-time-identity.md), a wrapping [digital counter](../../../../../digital-counter.md) is usable if elapsed-time subtraction is unsigned and the real observation interval is less than its modulus; a wide enough counter or suitable bounded intervals make this explicit. Software dispatch adds bounded latency, so the specification is achieved to timer/interrupt-service resolution; stricter physical pulse-width requirements call for hardware output comparison or a suitably prioritised timer handler.

Finally, the [device register](../../../../../device-register.md) is only a [single-bit event latch](../../../../../single-bit-event-latch.md). Two physical detections before acknowledgement may coalesce, so no software can recover their multiplicity from that [bit](../../../../../bit.md) alone. The [event counter](../../../../../event-counter.md) must also have enough capacity for the allowed backlog; indefinitely many arrivals faster than one flash every two seconds cannot be guaranteed with finite storage. These are explicit hardware/rate assumptions, not missing input files. Keeping the handler short minimises the rearming interval but cannot abolish those limitations.

## ↑ Ancestors (12)

1. [A](../a.md)
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
