# Bus ownership

↑ **Parent:** [Bus arbitration](bus-arbitration.md)

The permission to use a particular [computer bus](computer-bus.md) resource during a specified phase. A pending grant need not authorize immediate use. Arm's [AMBA Specification, revision 2.0](https://documentation-service.arm.com/static/642569a2314e245d086bc87e) (section 3.11.3, figures 3-15–3-17) makes address-path handover depend on completion, and delays [data bus](data-bus.md) ownership relative to [address bus](address-bus.md) ownership. Consequently, a single whole-[bus transaction](bus-transaction.md) owner is a useful simple model, but does not describe every overlapping implementation.

## ↑ Ancestors (4)

1. [Bus arbitration](bus-arbitration.md)
2. [Computer bus](computer-bus.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Bus burst](bus-burst.md)
- [Bus wait state](bus-wait-state.md)
- [Computer bus](computer-bus.md)
