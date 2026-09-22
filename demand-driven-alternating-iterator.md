# Demand-driven alternating iterator

↑ **Parent:** [Iterator](iterator.md)

A wrapper selecting alternate underlying entries can maintain one flag indicating whether the next entry must first be discarded. Construction performs no requests. On demand, skip at most that one entry, clear the flag, and leave the selected entry unconsumed until next is called. Returning a selected entry sets the flag again. Repeated availability tests cannot repeatedly skip; a final skipped entry may need to be consumed to establish exhaustion.

## ↑ Ancestors (4)

1. [Iterator](iterator.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
