# Scheduling waiting time

↑ **Parent:** [Process scheduling](process-scheduling.md)

The total duration a task spends runnable but waiting for a [CPU](central-processing-unit.md), including later waits after [scheduling preemption](scheduling-preemption.md). Under the zero-overhead, no-[input-output](input-output.md)-blocking assumptions of [process scheduling](process-scheduling.md), elapsed time partitions into useful execution and such waiting, so $W_i=T_i-b_i$, where $T_i$ is [scheduling turnaround time](scheduling-turnaround-time.md) and $b_i$ is the total [CPU burst](cpu-burst.md). Thus C under [round-robin scheduling](round-robin-scheduling.md) has $W_C=3-1=2$. If a task also spends time blocked on [input-output](input-output.md), that blocked duration belongs to [scheduling turnaround time](scheduling-turnaround-time.md) but must not be counted as [scheduling waiting time](scheduling-waiting-time.md).

// Target: computer-science.bigb

## ↑ Ancestors (4)

1. [Process scheduling](process-scheduling.md)
2. [Operating system](operating-system.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Process scheduling](process-scheduling.md)
- [Scheduling waiting time](scheduling-waiting-time.md)
