# Polled input-output

↑ **Parent:** [Operating system](operating-system-split.md)

In [polled input-output](polled-input-output.md), the [CPU](central-processing-unit.md) explicitly checks a device's status to discover whether work is ready or an operation has completed. Repeatedly checking in a tight loop is busy polling; periodic checks can instead leave time for other work. [Interrupt-driven input-output](interrupt-driven-input-output.md) changes how readiness is discovered, while [DMA](direct-memory-access.md) changes how payload data moves. [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 36, sections 36.3–36.5: polling, interrupts and DMA](https://pages.cs.wisc.edu/~remzi/OSTEP/file-devices.pdf)

Use the model drawn under [interrupt-driven input-output](interrupt-driven-input-output.md): device events occur at times $2,5,9$, while polls occur at $0,2,4,6,8,10,12$. Assume each event remains pending until detected and an event simultaneous with a poll is visible to that poll. The detection times are $2,6,10$, giving delays $0,1,1$. Four of the seven checks find no new event. These are event-detection delays, not completion times for servicing the events.

More generally, for polls at $0,\Delta,2\Delta,\ldots$ with $\Delta>0$, an event at time $t\geq0$ is first detected at

$$
d(t)=\Delta\left\lceil\frac{t}{\Delta}\right\rceil,\qquad 0\leq d(t)-t<\Delta.
$$

The [ceiling function](ceiling-function.md) chooses the first poll at or after the event. To verify the bound, that poll is less than one interval beyond $t$; if $t$ is itself a poll time, the delay is zero by the stated visibility convention. This argument assumes instantaneous checks, persistent pending status and an uninterrupted poll schedule. It does not describe missed transient events or a [CPU](central-processing-unit.md) too busy to maintain that schedule.

The attraction of [polled input-output](polled-input-output.md) is simple control and the possibility of processing several ready items in one visit. Busy polling spends [CPU](central-processing-unit.md) time even when nothing is ready, but short waits or frequent events can make avoiding repeated [interrupt](interrupt.md) entry worthwhile. The right choice depends on actual checking, notification and service costs. See [interrupt-driven input-output](interrupt-driven-input-output.md) for a documented combination of both strategies. [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 36, section 36.4: polling and interrupt tradeoffs](https://pages.cs.wisc.edu/~remzi/OSTEP/file-devices.pdf)

// Destination: computer-science.bigb

## ↑ Ancestors (3)

1. [Operating system](operating-system-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Central processing unit](central-processing-unit.md)
- [Device driver](device-driver.md)
- [Direct memory access](direct-memory-access.md)
- [Input-output](input-output.md)
- [Interrupt-driven input-output](interrupt-driven-input-output.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/8/a/ii/solution.md)
- [Polled input-output](polled-input-output.md)
